
<script>
import AppNavbar from "./components/appNavbar.vue";
import AppBanner from "./components/AppBanner.vue";
import AppHero from "./components/AppHero.vue";
import AppMain from "./components/appMain.vue";
import AppFooter from "./components/appFooter.vue";
import AppCta from "./components/appCta.vue";

export default {
  components: {
    AppNavbar,
    AppBanner,
    AppHero,
    AppMain,
    AppFooter,   
    AppCta,
    
},
  data() {
    return {
    
    }
  }
}
</script>

<template>

<AppNavbar />
<AppBanner />
<AppHero />
<AppMain />
<AppFooter />
<AppCta />

</template>

<style lang="scss">

//sass

@use "./style/general.scss"

</style>
