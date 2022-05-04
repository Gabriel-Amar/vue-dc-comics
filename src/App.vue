<template>
  <div id="app">

    <app-header/>

    <app-grid/>

    <app-main/>

    <app-links/>

    <app-footer/>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue"
import AppGrid from "./components/AppGrid.vue"
import AppMain from "./components/AppMain.vue"
import AppLinks from './components/AppLinks.vue'
import AppFooter from "./components/AppFooter.vue"
export default {
  name: 'App',
  components: {
    AppHeader,
    AppGrid,
    AppMain,
    AppLinks,
    AppFooter,
  }
}
</script>

<style lang="scss">
  @import "./style/variables";
  @import "./style/general";

</style>
