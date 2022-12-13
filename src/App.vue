<script>
import AppHeader from './components/header/AppHeader.vue';
import AppFooter from './components/footer/AppFooter.vue';
import AppMain from './components/main_content/AppMain.vue';


export default{
  components: {
    AppHeader,
    AppMain,
    AppFooter,
  },
}
</script>

<template>
  <AppHeader/>
  <AppMain/>
  <AppFooter/>
</template>

<style lang="scss">
  *{
    box-sizing: border-box;
  }

</style>
