<template>
  <Start />
  <PartnersPage/>
  <Features />
  <Testimonials />
  <SubscriptionPage />
  <FAQPage />
  <Footer />

</template>

<script>
import Start from './components/InitialPage.vue';
import Testimonials from './components/TestimonialsPage.vue';
import Features from './components/FeaturesPage.vue';
import Footer from './components/FooterPage.vue';
import FAQPage from './components/FAQPage.vue';
import PartnersPage from './components/PartnersPage.vue'
import SubscriptionPage from './components/SubscriptionPage.vue';

export default {
  name: 'App',
  components: {
    Start,
    Testimonials,
    Features,
    Footer,
    FAQPage,
    PartnersPage,
    SubscriptionPage,
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

a, a:visited {
  text-decoration: none;
  color: black;
}

.logo{
  height: 56px;
}

.title {
  font-size: x-large;
  color: black;
  text-align: center;
  padding-top: 3em;
}
</style>
