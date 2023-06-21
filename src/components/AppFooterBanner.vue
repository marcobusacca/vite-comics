<!-- SCRIPT VUE.JS -->
<script>
export default {
    data() {
        return {
            bannerItem: [
                {
                    label: 'DIGITAL COMICS',
                    src: '/src/assets/buy-comics-digital-comics.png',
                },
                {
                    label: 'DC MERCHANDISE',
                    src: '/src/assets/buy-comics-merchandise.png',
                },
                {
                    label: 'SUBSCRIPTION',
                    src: '/src/assets/buy-comics-subscriptions.png',
                },
                {
                    label: 'COMICS SHOP LOCATOR',
                    src: '/src/assets/buy-comics-shop-locator.png',
                },
                {
                    label: 'DC POWER VISA',
                    src: '/src/assets/buy-dc-power-visa.svg',
                },
            ]
        }
    },
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
                <div class="banner-col" v-for="(item, index) in bannerItem" :key="index">
                    <!-- Banner Image -->
                    <img :src="item.src" :alt="`banner-image-${index+1}`">
                    <!-- Banner Text -->
                    <span v-text="item.label"></span>
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