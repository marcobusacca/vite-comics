<!-- SCRIPT VUE.JS -->
<script>
export default {
    data() {
        return {

        }
    },
}
</script>

<!-- TEMPLATE HTML -->
<template lang="">
    <footer>
        <!-- Footer Banner Container Fluid -->
        <div class="container-fluid banner-container">
            <!-- Footer Banner Container -->
            <div class="container">
                <!-- Footer Banner Row -->
                <div class="row">
                    <!-- Footer Banner Col -->
                    <div class="col">
                        <!-- Banner Sub Row -->
                        <div class="row">
                            <!-- Banner Sub Col -->
                            <div class="banner-col"></div>
                            <div class="banner-col"></div>
                            <div class="banner-col"></div>
                            <div class="banner-col"></div>
                            <div class="banner-col"></div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- Footer Menu Container Fluid -->
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
                            <div class="menu-col"></div>
                            <div class="menu-col"></div>
                            <div class="menu-col"></div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- Footer Bottom Bar Container Fluid -->
        <div class="container-fluid bottom-bar-container">
            <!-- Footer Bottom Bar Container -->
            <div class="container">
                <!-- Footer Bottom Bar Row -->
                <div class="row">
                    <!-- Footer Bottom Bar Col -->
                    <div class="col">
                        <!-- Bottom Bar Sub Row -->
                        <div class="row">
                            <!-- Bottom Bar Sub Col -->
                            <div class="bottom-bar-col"></div>
                            <div class="bottom-bar-col"></div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<!-- STYLE SCSS -->
<style lang="scss" scoped>
footer {
    width: 100%;
    height: calc(100% - 350px);
    background-color: blue;

    .container-fluid {
        width: 100%;
        height: calc(100% / 3);
        padding: 10px 20px;
        background-color: yellow;
        border: 1px solid black;

        .container {
            background-color: red;
            max-width: 1600px;
            margin: 0 auto;
            height: 100%;

            .row {
                display: flex;
                flex-wrap: wrap;
                height: 100%;

                .col {
                    width: 100%;
                    height: 100%;
                    border: 2px dashed black;
                    padding: 10px;
                }

                .banner-col {
                    width: calc(100% / 5);
                    height: 100%;
                    border: 1px solid #fff;
                }

                .menu-col {
                    width: calc(100% / 3);
                    height: 100%;
                    border: 1px solid #fff;
                }

                .bottom-bar-col {
                    width: calc(100% / 2);
                    height: 100%;
                    border: 1px solid #fff;
                }
            }
        }
    }

    .banner-container {
        background-color: #0282F9;
    }

    .menu-container {
        background-image: url(../assets/footer-bg.jpg);
    }

    .bottom-bar-container {
        background-color: #303030;
    }
}
</style>