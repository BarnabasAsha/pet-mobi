<template>
  <Header />
  <main>
    <Hero />
    <Featured />
    <FlexWrapper />
    <Schedule />
    <Testimonials />
    <Doggies />
    <Download />
    <Footer />
  </main>
</template>

<script>
import Header from "./components/Header.vue";
import Hero from "./components/Hero.vue";
import Featured from "./components/Featured.vue";
import Schedule from "./components/Schedule.vue";
import FlexWrapper from "./components/FlexWrapper.vue";
import Testimonials from "./components/Testimonials.vue";
import Doggies from "./components/Doggies.vue";
import Download from "./components/Download.vue";
import Footer from "./components/Footer/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Hero,
    Featured,
    Schedule,
    FlexWrapper,
    Testimonials,
    Doggies,
    Download,
    Footer,
  },
};
</script>

<style lang="scss" src="./styles/app.scss"></style>
