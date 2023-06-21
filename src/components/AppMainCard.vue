<!-- SCRIPT VUE.JS -->
<script>
export default {
    props: {
        thumb: String,
        series: String,
    }
}
</script>

<!-- TEMPLATE HTML -->
<template lang="">
    <!-- Main Content Card Col -->
    <div class="card-col">
        <!-- Card Image -->
        <div class="card-image" :style="`background-image: url('${thumb}')`">
        </div>
        <!-- Card Text -->
        <div class="card-text">
            <h3 v-text="series.toUpperCase()"></h3>
        </div>
    </div>
</template>

<!-- STYLE SCSS -->
<style lang="scss" scoped>
// IMPORTO IL FILE _VARIABLES.SCSS
@use '../styles/partials/variables' as *;

.card-col {
    width: calc(100% / 6 - 40px);
    margin: 20px;

    .card-image {
        width: 235px;
        height: 235px;
        background-size: cover;
        cursor: pointer;

        &:hover {
            border: 4px solid $secondaryColor;
        }
    }

    .card-text {
        font-size: 13px;
        padding: 20px 0;
        cursor: pointer;

        h3:hover {
            text-shadow: 0 0 10px $secondaryColor;
        }
    }
}
</style>