<template>
    <div :class="containerClass">
    </div>
</template>

<script>
import EventBus from '@/AppEventBus';

export default {
    props: {
        theme: String,
        inputStyle: String
    },
    data() {
        return {
            active: false,
            scale: 14,
            scales: [12,13,14,15,16]
        }
    },
    outsideClickListener: null,
    themeChangeListener: null,
    watch: {
        $route() {
            if (this.active) {
                this.active = false;
                this.unbindOutsideClickListener();
            }
        }
    },
    beforeUnmount() {
        EventBus.off('change-theme', this.themeChangeListener);
    },
    mounted() {
        this.themeChangeListener = (event) => {
            if (event.theme === 'nano')
                this.scale = 12;
            else
                this.scale = 14;

            this.applyScale();
        };

        EventBus.on('change-theme', this.themeChangeListener);
    },
    methods: {
        toggleConfigurator(event) {
            this.active = !this.active;
            event.preventDefault();

            if (this.active)
                this.bindOutsideClickListener();
            else
                this.unbindOutsideClickListener();
        },
        hideConfigurator(event) {
            this.active = false;
            this.unbindOutsideClickListener();
            event.preventDefault();
        },
        changeTheme(event, theme, dark) {
            this.$emit('change-theme', {theme: theme, dark: dark});
            event.preventDefault();
        },
        bindOutsideClickListener() {
            if (!this.outsideClickListener) {
                this.outsideClickListener = (event) => {
                    if (this.active && this.isOutsideClicked(event)) {
                        this.active = false;
                    }
                };
                document.addEventListener('click', this.outsideClickListener);
            }
        },
        unbindOutsideClickListener() {
            if (this.outsideClickListener) {
                document.removeEventListener('click', this.outsideClickListener);
                this.outsideClickListener = null;
            }
        },
        isOutsideClicked(event) {
            return !(this.$el.isSameNode(event.target) || this.$el.contains(event.target));
        },
        decrementScale() {
            this.scale--;
            this.applyScale();
        },
        incrementScale() {
            this.scale++;
            this.applyScale();
        },
        applyScale() {
            document.documentElement.style.fontSize = this.scale + 'px';
        },
        onRippleChange(value) {
            this.$primevue.config.ripple = value;
        }
    },
    computed: {
        containerClass() {
            return ['layout-config', {'layout-config-active': this.active}];
        },
        rippleActive() {
            return this.$primevue.config.ripple;
        }
    }
}
</script>
