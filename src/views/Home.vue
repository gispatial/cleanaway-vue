<template>
    <div class="home">
        <div :class="introductionClass">
            <div class="introduction-promo"><h1>With you, for you -<br> Essential waste and<br> resource recovery services</h1></div>
            <div class="introduction-promo">Solutions for your industry</div>
           <p></p>
            <router-link to="/setup" class="action-button">GET STARTED</router-link>
            <img alt="devices" class="introduction-devices" src="../assets/images/home/intro-devices.png" />
        </div>

        <div class="whouses">
            <h4>Investing in our future</h4>
            <p>Our shareholders play a big part in making a sustainable future possible. In this section, we present links to all our market-sensitive company information, news and current share price details. Our “Introduction to Cleanaway” presentation provides a useful overview of the business and industry. Key historical financial performance data for Cleanaway can be downloaded in spreadsheet format here. Cleanaway Waste Management Limited is Australia’s leading waste management company,.</p>
            <div class="p-grid">
                <div class="p-col-6 p-md-2"><img alt="airbus" src="../assets/images/home/airbus.svg"/></div>
                <div class="p-col-6 p-md-2"><img alt="amex" src="../assets/images/home/amex.svg"/></div>
                <div class="p-col-6 p-md-2"><img alt="bmw" src="../assets/images/home/nvidia.svg"/></div>
                <div class="p-col-6 p-md-2"><img alt="ebay" src="../assets/images/home/ebay.svg"/></div>
                <div class="p-col-6 p-md-2"><img alt="ford" src="../assets/images/home/ford.svg"/></div>
                <div class="p-col-6 p-md-2"><img alt="fox" src="../assets/images/home/fox.svg"/></div>
                <div class="p-col-6 p-md-2"><img alt="lufthansa" src="../assets/images/home/lufthansa.svg"/></div>
                <div class="p-col-6 p-md-2"><img alt="mercedes" src="../assets/images/home/mercedes.svg"/></div>
                <div class="p-col-6 p-md-2"><img alt="sap" src="../assets/images/home/sap.svg"/></div>
                <div class="p-col-6 p-md-2"><img alt="unicredit" src="../assets/images/home/unicredit.svg"/></div>
                <div class="p-col-6 p-md-2"><img alt="verizon" src="../assets/images/home/verizon.svg"/></div>
                <div class="p-col-6 p-md-2"><img alt="viacom" src="../assets/images/home/viacom.svg"/></div>
            </div>
        </div>

        <div class="features">
            <h4>About Cleanaway</h4>
            <p>Sustainability is at the core of everything we do. We strive to make a sustainable future possible for everyone, from our customers and employees to our shareholders and the community. Our entire operations are focused on delivering sustainability in these five key areas, with an eye on the triple bottom line of sustainability – the environment, society and the economy.</p>

            <div class="p-grid">
                <div class="p-col-12 p-md-4">
                    <div class="feature-card">
                        <img alt="components" src="../assets/images/home/vue-components.png" />
                        <div class="feature-card-detail">
                            <div class="feature-name">80+ COMPONENTS</div>
                            <p>The ultimate set of UI Components to assist you with 80+ impressive Vue Components.</p>
                        </div>
                    </div>
                </div>
                <div class="p-col-12 p-md-4">
                    <div class="feature-card">
                        <img alt="opensource" src="../assets/images/home/vue-opensource.png" />
                        <div class="feature-card-detail">
                            <div class="feature-name">OPEN SOURCE</div>
                            <p>The complete UI Suite is free to based on the MIT license and the source code is available at GitHub.</p>
                        </div>
                    </div>
                </div>
                <div class="p-col-12 p-md-4">
                    <div class="feature-card">
                        <img alt="themes" src="../assets/images/home/vue-themes.png" />
                        <div class="feature-card-detail">
                            <div class="feature-name">THEMES</div>
                            <p>Build on a design-agnostic api, choose from a vast amount of themes such as material, bootstrap, custom or develop your own.</p>
                        </div>
                    </div>
                </div>
                <div class="p-col-12 p-md-4">
                    <div class="feature-card">
                        <img alt="templates" src="../assets/images/home/vue-templates.png" />
                        <div class="feature-card-detail">
                            <div class="feature-name">TEMPLATES</div>
                            <p>Fascinating Vue-CLI application templates designed by professional designers and crafted by Vue Experts.</p>
                        </div>
                    </div>
                </div>
                <div class="p-col-12 p-md-4">
                    <div class="feature-card">
                        <img alt="accesibility" src="../assets/images/home/vue-accesibility.png" />
                        <div class="feature-card-detail">
                            <div class="feature-name">ACCESSIBILITY</div>
                            <p>UI Components for everyone with full support for Web Content Accessibility Guidelines (WCAG).</p>
                        </div>
                    </div>
                </div>
                <div class="p-col-12 p-md-4">
                    <div class="feature-card">
                        <img alt="pro" src="../assets/images/home/vue-pro.png" />
                        <div class="feature-card-detail">
                            <div class="feature-name">PRO SUPPORT</div>
                            <p>Exceptional support service featuring response within 1 business day and option to request enhancements and new features for the library.</p>
                        </div>
                    </div>
                </div>
                <div class="p-col-12 p-md-4">
                    <div class="feature-card">
                        <img alt="productivity" src="../assets/images/home/vue-productivity.png" />
                        <div class="feature-card-detail">
                            <div class="feature-name">PRODUCTIVITY</div>
                            <p>Boost your productivity by achieving more in less time and accomplish amazing results.</p>
                        </div>
                    </div>
                </div>
                <div class="p-col-12 p-md-4">
                    <div class="feature-card">
                        <img alt="community" src="../assets/images/home/vue-community.png" />
                        <div class="feature-card-detail">
                            <div class="feature-name">COMMUNITY</div>
                            <p>Connect with the other open source community members, collaborate and have a voice in the project roadmap.</p>
                        </div>
                    </div>
                </div>


                <div class="p-col-12 p-md-4">
                    <div class="feature-card">
                        <img alt="mobile" src="../assets/images/home/vue-mobile.png" />
                        <div class="feature-card-detail">
                            <div class="feature-name">MOBILE</div>
                            <p>First class support for responsive design led by touch optimized elements.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div class="primeflex">
            <div class="p-grid">
                <div class="p-col-12 p-md-6">
                    <h3 class="pro-title">General Waste and Recycling: Services</h3>
                    <p>Businesses can divert more waste from landfill and improve sustainability rates with tailored general waste and recycling management.</p>
                    <a class="action-button" href="https://www.primefaces.org/primeflex">LEARN MORE</a>
                </div>
                <div class="p-col-12 p-md-6 p-text-center">
                    <img alt="primeflex" src="../assets/images/primeflex.png" class="section-image">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import EventBus from '@/AppEventBus';

export default {
    data() {
        return {
            dark: false
        }
    },
    themeChangeListener: null,
    mounted() {
        let afId = this.$route.query['af_id'];
        if (afId) {
            let today = new Date();
            let expire = new Date();
            expire.setTime(today.getTime() + 3600000*24*7);
            document.cookie = 'primeaffiliateid=' + afId + ';expires=' + expire.toUTCString() + ';path=/; domain:primefaces.org';
        }

        this.themeChangeListener = (event) => {
            if (event.dark)
                this.dark = true;
            else
                this.dark = false;
        };
        EventBus.on('change-theme', this.themeChangeListener);
    },
    beforeUnmount() {
        EventBus.off('change-theme', this.themeChangeListener);
    },
    computed: {
        introductionClass() {
            return ['introduction', {'introduction-dark': this.dark}];
        }
    }
}
</script>
