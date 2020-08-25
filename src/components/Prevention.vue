<template>
  <div id="prevention" class="prevention">
    <h2>Prevention</h2>
    <div class="prevention-section">
      <div class="prevention-content">
        <h2>
          7 steps to prevent
          <br />the spread of
          <br />covid 19.
        </h2>
        <ul>
          <li>
            <span>01.</span>
            <p>Wash your hands frequently</p>
          </li>
          <li>
            <span>02.</span>
            <p>Avoid touching your eyes, nose, and mouth</p>
          </li>
          <li>
            <span>03.</span>
            <p>Cover your mouth when you cough using a tissue or the bend of your elbow</p>
          </li>
          <li>
            <span>04.</span>
            <p>Avoid crowded places and close contact with anyone who has fever or cough</p>
          </li>
          <li>
            <span>05.</span>
            <p>Stay home if you feel unwell</p>
          </li>
          <li>
            <span>06.</span>
            Seek medical care early if you have afever, coughs, and difficulty breathing—but call first
          </li>
          <li>
            <span>07.</span>
            <p>Get information from trusted sources</p>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.prevention {
  h2 {
    color: #fff;
    font-size: 1.975rem;
    padding-bottom: 4rem;
  }
  .prevention-content {
    background: #f88949;
    display: flex;
    flex-direction: row;
    justify-content: center;
    flex-wrap: wrap;
    // align-items: center;
    padding: 3.125rem 2rem;
    margin: 0 auto;

    h2 {
      font-size: 5rem;
      line-height: 7rem;
      color: #242058;
      text-align: center;
      // width: 50%;
    }
    ul {
      display: flex;
      flex-direction: column;
      justify-content: center;
      // width: 50%;
      li {
        display: flex;
        flex-direction: row;
        // width: 65%;
        font-size: 2.2rem;
        line-height: 4.5rem;
        letter-spacing: 0.075rem;
        list-style: none;
        color: #fff;
        padding-bottom: 2rem;
        span {
          font-size: 4rem;
          line-height: 3.7rem;
          letter-spacing: 0.075rem;
          color: rgb(95, 94, 94);
          padding-right: 0.625em;
        }
        .white {
          color: #fff;
        }
      }
    }
  }
}
</style>