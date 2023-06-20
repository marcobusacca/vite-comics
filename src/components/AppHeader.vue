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
    <header>
        <!-- Header Container -->
        <div class="container">
            <!-- Header Row -->
            <div class="row">
                <!-- Header Logo Col -->
                <div class="col">
                    <!-- Header Logo -->
                </div>
                <!-- Header Menu Col -->
                <div class="col">
                    <!-- Header Menu -->
                </div>
            </div>
        </div>
    </header>
</template>

<!-- STYLE SCSS -->
<style lang="scss" scoped>
header {
    height: 150px;
    padding: 20px;
    background-color: blue;

    .container {
        background-color: red;
        max-width: 1800px;
        margin: 0 auto;
        height: 100%;

        .row {
            display: flex;
            height: 100%;

            .col {
                width: calc(100% / 2);
                height: 100%;
                border: 1px dashed black;
            }
        }
    }
}
</style>