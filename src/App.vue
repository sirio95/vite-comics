<script>
import Hero from './components/header/Hero.vue';
import BlueStripe from './components/footer/BlueStripe.vue';
import UsefulLinks from './components/footer/UsefulLinks.vue';
import Socials from './components/footer/Socials.vue';

export default{
  components: {
    Hero,
    BlueStripe,
    UsefulLinks,
    Socials,
  }
}
</script>

<template>
  <Hero/>
  <BlueStripe/>
  <UsefulLinks/>
  <Socials/>
</template>

<style scoped>

</style>
