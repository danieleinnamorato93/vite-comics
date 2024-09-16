<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppMidNav from './components/AppMidNav.vue';
import AppSectionLinks from './components/AppSectionLinks.vue';
import AppFooter from './components/AppFooter.vue';
export default {
  data() {
    return{

    };
  
  },

components: {AppHeader,
AppMain,
AppMidNav,
AppSectionLinks,
AppFooter}
};
</script>

<template>
  <AppHeader/>
  <AppMain/>
  <AppMidNav/>
  <AppSectionLinks/>
  <AppFooter/>
</template>
<style lang="scss">
@use"./styles/general.scss" as *;
</style>