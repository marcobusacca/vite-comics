<!-- SCRIPT VUE.JS -->
<script>
export default {

}
</script>

<!-- TEMPLATE HTML -->
<template lang="">
    <!-- Footer Banner -->
    <div class="container-fluid banner-container">
        <!-- Footer Banner Container -->
        <div class="container">
            <!-- Banner Row -->
            <div class="row">
                <!-- Banner Col -->
                <div class="banner-col">
                    <!-- Banner Image -->
                    <img src="../assets/buy-comics-digital-comics.png" alt="banner-image-1">
                    <!-- Banner Text -->
                    <span>DIGITAL COMICS</span>
                </div>
                <!-- Banner Col -->
                <div class="banner-col">
                    <!-- Banner Image -->
                    <img src="../assets/buy-comics-merchandise.png" alt="banner-image-2">
                    <!-- Banner Text -->
                    <span>DC MERCHANDISE</span>
                </div>
                <!-- Banner Col -->
                <div class="banner-col">
                    <!-- Banner Image -->
                    <img src="../assets/buy-comics-subscriptions.png" alt="banner-image-3">
                    <!-- Banner Text -->
                    <span>SUBSCRIPTION</span>
                </div>
                <!-- Banner Col -->
                <div class="banner-col">
                    <!-- Banner Image -->
                    <img src="../assets/buy-comics-shop-locator.png" alt="banner-image-4">
                    <!-- Banner Text -->
                    <span>COMICS SHOP LOCATOR</span>
                </div>
                <!-- Banner Col -->
                <div class="banner-col">
                    <!-- Banner Image -->
                    <img src="../assets/buy-dc-power-visa.svg" alt="banner-image-5">
                    <!-- Banner Text -->
                    <span>DC POWER VISA</span>
                </div>
            </div>
        </div>
    </div>
</template>

<!-- STYLE SCSS -->
<style lang="scss" scoped>
// IMPORTO IL FILE _VARIABLES.SCSS
@use '../styles/partials/variables' as *;

.banner-col {
    display: flex;
    justify-content: center;
    align-items: center;
    width: calc(100% / 5 - 40px);
    margin: 0 20px;
    height: 100%;

    img {
        width: 20%;

        &:hover {
            filter: invert(100%);
        }
    }

    span {
        margin-left: 20px;
        font-size: 15px;

        &:hover {
            color: black;
            font-weight: 700;
        }
    }

    img,
    span {
        cursor: pointer;
    }
}

.banner-container {
    height: 160px;
    background-color: $secondaryColor;
}
</style>