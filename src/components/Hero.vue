<template>
  <div class="hero">
    <div class="hero-content">
      <h1>
        getting you
        <span id="orange">informed</span> on
        <span id="white">covid-19</span>
        <span id="orange">.</span>
      </h1>
      <!-- <img src="../assets/doctor.svg" alt="doctors svg" /> -->
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.hero-content {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 70vh;
  h1 {
    // width: 40%;
    font-size: 7rem;
    line-height: 10rem;
    letter-spacing: 0.015em;
    color: #242058;
    #orange {
      color: #f88949;
    }
    #white {
      color: #ffffff;
    }
  }
  img {
    // height: 600px;
    margin: 0 auto;
    width: 60%;
  }
}
</style>