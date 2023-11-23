
<script>
import AppNavbar from "./components/appNavbar.vue";
import Apphero from "./components/appHero.vue";
import AppMain from "./components/appMain.vue";
import AppFooter from "./components/appFooter.vue";
import AppCta from "./components/appCta.vue";

export default {
  components: {
    AppNavbar,
    Apphero,
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
<Apphero />
<AppMain />
<AppFooter />
<AppCta />

</template>

<style lang="scss">

//sass
@use "src/style/general.scss"

</style>
