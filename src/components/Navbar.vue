<template>
  <div class="navigation">
    <h1>
      covid-19 info
      <span>hub</span>
    </h1>
    <ul>
      <li>
        <a href="#tracker">Tracker</a>
      </li>
      <li>
        <a href="#prevention">Prevention</a>
      </li>
      <li>
        <a href="#symptoms">Symptoms</a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.navigation {
  display: flex;
  flex-direction: row;
  justify-content: center;
  flex-wrap: wrap;
  align-items: center;
  height: 12vh;
  padding: 0 2.5rem;
  h1 {
    font-size: 3rem;
    color: #242058;
    letter-spacing: 0.015em;
    span {
      color: #f88949;
    }
  }
  ul {
    display: flex;
    flex-direction: row;
    li {
      list-style: none;
      margin-left: 1.5rem;
      padding: 0.5rem;
      text-align: center;
      border-bottom: 2px solid #f88949;
      a {
        color: #000;
        text-decoration: none;
        font-size: 2rem;
        letter-spacing: 0.2rem;
        &:hover {
          color: #fff;
        }
      }
    }
  }
}
</style>