<template>
  <div id="symptoms" class="symptoms">
    <h2 class="label">symptoms</h2>
    <div class="symptoms-content">
      <h2>
        lookout for the following
        <span>symptoms</span>
      </h2>
      <div class="symptoms-list">
        <ul>
          <li>Fever</li>
          <li>Cough</li>
          <li>Vomiting</li>
          <li>Headache</li>
          <li>dizziness</li>
          <li>Sore throat</li>
          <li>Shortness of breathe</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.symptoms {
  padding: 4rem 0;

  .label {
    color: #fff;
    font-size: 1.975rem;
    padding: 4rem 0;
  }
  .symptoms-content {
    h2 {
      text-align: center;
      font-size: 2.6rem;
      padding: 1rem;
      color: #ffff;
      padding-bottom: 3rem;
      span {
        color: #f88949;
        text-decoration: underline;
      }
    }
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    flex-wrap: wrap;
    align-items: center;
    padding-top: 3.125rem;

    .symptoms-list {
      margin: 0 auto;
      ul {
        li {
          font-size: 2.2rem;
          line-height: 3.5rem;
          letter-spacing: 0.075em;
          list-style: none;
          color: #24285b;
          text-align: center;
        }
      }
    }
  }
}
</style>