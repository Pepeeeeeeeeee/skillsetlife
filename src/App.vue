<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <Start />
  <PartnersPage/>
  <Intro />
  <Testimonials />
  <Process />
  <FAQPage />
  <Footer />

</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import Testimonials from './components/TestimonialsPage.vue';
import Process from './components/ProcessPage.vue';
import Start from './components/InitialPage.vue';
import Intro from './components/IntroPage.vue';
import Footer from './components/FooterPage.vue';
import FAQPage from './components/FAQPage.vue';
import PartnersPage from './components/PartnersPage.vue'

export default {
  name: 'App',
  components: {
    //HelloWorld
    Testimonials,
    Process,
    Start,
    Intro,
    Footer,
    FAQPage,
    PartnersPage
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
