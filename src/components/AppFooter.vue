<!-- SCRIPT VUE.JS -->
<script>
// IMPORTO APP_FOOTER_BANNER
import AppFooterBanner from './AppFooterBanner.vue';

export default {
    components: {
        // DICHIARO APP_FOOTER_BANNER
        AppFooterBanner
    },
}
</script>

<!-- TEMPLATE HTML -->
<template lang="">
    <footer>
        <!-- Footer Banner -->
        <AppFooterBanner/>
        <!-- Footer Menu -->
        <div class="container-fluid menu-container">
            <!-- Footer Menu Container -->
            <div class="container">
                <!-- Footer Menu Row -->
                <div class="row">
                    <!-- Footer Menu Col -->
                    <div class="col">
                        <!-- Menu Sub Row -->
                        <div class="row">
                            <!-- Menu Sub Col -->
                            <div class="menu-col">
                                <!-- List Title -->
                                <h3>DC COMICS</h3>
                                <!-- Menu List -->
                                <ul>
                                    <li>
                                        <a href="#">Characters</a>
                                    </li>
                                    <li>
                                        <a href="#">Comics</a>
                                    </li>
                                    <li>
                                        <a href="#">Movies</a>
                                    </li>
                                    <li>
                                        <a href="#">TV</a>
                                    </li>
                                    <li>
                                        <a href="#">Games</a>
                                    </li>
                                    <li>
                                        <a href="#">Videos</a>
                                    </li>
                                    <li>
                                        <a href="#">News</a>
                                    </li>
                                </ul>
                                <!-- List Title -->
                                <h3>SHOP</h3>
                                <!-- Menu List -->
                                <ul>
                                    <li>
                                        <a href="#">Shop DC</a>
                                    </li>
                                    <li>
                                        <a href="#">Shop DC Collectibles</a>
                                    </li>
                                </ul>
                            </div>
                            <div class="menu-col">
                                <!-- List Title -->
                                <h3>DC</h3>
                                <!-- Menu List -->
                                <ul>
                                    <li>
                                        <a href="#">Terms Of Use</a>
                                    </li>
                                    <li>
                                        <a href="#">Privacy policy (New)</a>
                                    </li>
                                    <li>
                                        <a href="#">Ad Choices</a>
                                    </li>
                                    <li>
                                        <a href="#">Advertising</a>
                                    </li>
                                    <li>
                                        <a href="#">Jobs</a>
                                    </li>
                                    <li>
                                        <a href="#">Subscriptions</a>
                                    </li>
                                    <li>
                                        <a href="#">Talent Workshops</a>
                                    </li>
                                    <li>
                                        <a href="#">CPSC Certificates</a>
                                    </li>
                                    <li>
                                        <a href="#">Ratings</a>
                                    </li>
                                    <li>
                                        <a href="#">Shop Help</a>
                                    </li>
                                    <li>
                                        <a href="#">Contact Us</a>
                                    </li>
                                </ul>
                            </div>
                            <div class="menu-col">
                                <!-- List Title -->
                                <h3>SITES</h3>
                                <!-- Menu List -->
                                <ul>
                                    <li>
                                        <a href="#">DC</a>
                                    </li>
                                    <li>
                                        <a href="#">MAD Magazine</a>
                                    </li>
                                    <li>
                                        <a href="#">DC Kids</a>
                                    </li>
                                    <li>
                                        <a href="#">DC Universe</a>
                                    </li>
                                    <li>
                                        <a href="#">DC Power Visa</a>
                                    </li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    <!-- Footer Background Logo Col -->
                    <div class="col">
                        <!-- Background Logo Sub Row -->
                        <div class="row">
                            <!-- Background Logo Sub Col -->
                            <div class="background-logo-sub-col">
                                <!-- Background Logo -->
                                <img src="../assets/dc-logo-bg.png" alt="dc-background-logo">
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- Footer Bottom Bar -->
        <div class="container-fluid bottom-bar-container">
            <!-- Footer Bottom Bar Container -->
            <div class="container">
                <!-- Bottom Bar Row -->
                <div class="row">
                    <!-- Bottom Bar Col -->
                    <div class="bottom-bar-col">
                        <!-- Bottom Bar Sign Up Button -->
                        <a href="#" class="btn-sign-up">SIGN-UP NOW!</a>
                    </div>
                    <!-- Bottom Bar Col -->
                    <div class="bottom-bar-col">
                        <!-- Bottom Bar Follow Us -->
                        <h4>FOLLOW US</h4>
                        <!-- Facebook Link -->
                        <a href="#">
                            <img src="../assets/footer-facebook.png" alt="facebook-icon">
                        </a>
                        <!-- Twitter Link -->
                        <a href="#">
                            <img src="../assets/footer-twitter.png" alt="twitter-icon">
                        </a>
                        <!-- YouTube Link -->
                        <a href="#">
                            <img src="../assets/footer-youtube.png" alt="youtube-icon">
                        </a>
                        <!-- Pinterest Link -->
                        <a href="#">
                            <img src="../assets/footer-pinterest.png" alt="pinterest-icon">
                        </a>
                        <!-- Periscope Link -->
                        <a href="#">
                            <img src="../assets/footer-periscope.png" alt="periscope-icon">
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<!-- STYLE SCSS -->
<style lang="scss" scoped>
// IMPORTO IL FILE _VARIABLES.SCSS
@use '../styles/partials/variables' as *;

footer {
    width: 100%;
    background-color: blue;
    color: $primaryColor;

    .container-fluid {
        padding: 10px 20px;

        .row {
            padding: 10px;

            .col {
                width: calc(100% / 2);
            }

            .menu-col {
                height: 100%;
                margin-right: 50px;

                h3 {
                    margin: 15px 0px;
                }

                li {
                    padding: 5px 0px;
                    color: #959595;

                    a:hover {
                        color: $primaryColor;
                    }
                }
            }

            .background-logo-sub-col {
                display: flex;
                justify-content: center;
                align-items: center;
                position: relative;
                width: 100%;
                padding-top: 100px;

                img {
                    position: absolute;
                    width: 100%;
                }
            }

            .bottom-bar-col {
                display: flex;
                align-items: center;
                width: calc(100% / 2 - 50px);
                height: 100%;

                .btn-sign-up {
                    padding: 15px 10px;
                    font-weight: 700;
                    border: 4px solid $secondaryColor;
                    transition: all 1s;

                    &:hover {
                        background-color: #fff;
                        color: black;
                    }
                }

            }

            .bottom-bar-col:last-child {
                justify-content: flex-end;

                h4 {
                    margin: 0 20px;
                    font-size: 17px;
                    color: $secondaryColor;
                }

                a {
                    padding: 0px 10px;

                    &:hover img {
                        filter: brightness(1000%);
                    }
                }
            }
        }
    }

    .menu-container {
        background-image: url(../assets/footer-bg.jpg);
        background-size: cover;
        overflow-y: hidden;
        padding-bottom: 150px;
    }

    .bottom-bar-container {
        background-color: #303030;

        .row {
            align-items: center;
        }
    }
}
</style>