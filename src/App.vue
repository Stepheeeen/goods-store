<template>
  <NavBar navName="Store"/>
  <HomePage />
  <SalePage />
  <ContactPage />
</template>

<script>
import NavBar from './components/NavBar.vue'
import HeroPage from './components/HeroPage.vue'
import SalePage from './components/SalePage.vue'
import ContactPage from './components/ContactPage.vue'
export default {
  components: {
    'NavBar': NavBar,
    'HomePage': HeroPage,
    'SalePage': SalePage,
    'ContactPage': ContactPage
  },
  data() {
    return {
      navName: " "
    };
  }
};


</script>

<style>
  *{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }
</style>