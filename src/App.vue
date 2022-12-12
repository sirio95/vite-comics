<script>
import Hero from './components/header/Hero.vue';
import BlueStripe from './components/footer/BlueStripe.vue';
import UsefulLinks from './components/footer/UsefulLinks.vue';

export default{
  components: {
    Hero,
    BlueStripe,
    UsefulLinks,
  }
}
</script>

<template>
  <Hero/>
  <BlueStripe/>
  <UsefulLinks/>
</template>

<style scoped>

</style>
