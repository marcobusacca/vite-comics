<!-- SCRIPT VUE.JS -->
<script>
// IMPORTO APP_HEADER
import AppHeader from './components/AppHeader.vue';

// IMPORTO APP_MAIN
import AppMain from './components/AppMain.vue';

// IMPORTO APP_FOOTER
import AppFooter from './components/AppFooter.vue';

export default {
  // DICHIARO APP_HEADER
  AppHeader,

  // DICHIARO APP_MAIN
  AppMain,

  // DICHIARO APP_FOOTER
  AppFooter,
}
</script>

<!-- TEMPLATE HTML -->
<template lang="">
    <AppHeader/>
    <AppMain/>
    <AppFooter/>
</template>

<!-- STYLE SCSS -->
<style lang="" scoped></style>