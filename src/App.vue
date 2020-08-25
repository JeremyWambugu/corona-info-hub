<template>
  <div id="app">
    <Navbar />
    <div class="container">
      <Hero />
      <StatisticsCard />
      <Prevention />
      <Symptoms />
      <Footer />
    </div>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Hero from "@/components/Hero.vue";
import StatisticsCard from "@/components/StatisticsCard.vue";
import Prevention from "@/components/Prevention.vue";
import Symptoms from "@/components/Symptoms.vue";
import Footer from "@/components/Footer.vue";
export default {
  name: "App",
  components: {
    Navbar,
    Hero,
    StatisticsCard,
    Prevention,
    Symptoms,
    Footer
  },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Staatliches", cursive;
}
#app {
  background: #83c9b5;
}
.container {
  width: 90%;
  margin: 0 auto;
  // display: flex;
  // flex-direction: column;
  // flex-wrap: wrap;
}
</style>
