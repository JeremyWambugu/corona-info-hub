<template>
  <div id="tracker" class="statistics">
    <h2>Tracker</h2>
    <div class="main-card">
      <h3 class="country-name">{{country}}</h3>
      <div class="primary-cards">
        <div class="secondary-card recovered">
          <h3>Recovered</h3>
          <span>{{recovered}}</span>
          <p>Number of recoveries in {{country}}</p>
        </div>
        <div class="secondary-card active">
          <h3>Active</h3>
          <span>{{active}}</span>
          <p>Number of active cases in {{country}}</p>
        </div>
        <div class="secondary-card deaths">
          <h3>Deaths</h3>
          <span>{{deaths}}</span>
          <p>Number of deaths in {{country}}</p>
        </div>
      </div>
      <div class="search">
        <input type="text" placeholder="enter a country name" />
        <button>search</button>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  data() {
    return {
      country: "kenya",
      recovered: null,
      active: null,
      deaths: null,
    };
  },
  created() {
    axios(
      `https://covid-193.p.rapidapi.com/statistics?country=${this.country}`,
      {
        method: "GET",
        headers: {
          "x-rapidapi-host": "covid-193.p.rapidapi.com",
          "x-rapidapi-key":
            "441614529bmsh8c807c34709f5d2p165d8bjsnc13e4abebbe3",
        },
      }
    ).then((res) => {
      console.log(res.data.response[0].cases.recovered);
      this.active = res.data.response[0].cases.active;
      this.deaths = res.data.response[0].deaths.total;
      this.recovered = res.data.response[0].cases.recovered;
    });
  },
};
</script>

<style lang="scss" scoped>
.statistics {
  margin: 8rem 0;
  h2 {
    color: #fff;
    padding-bottom: 1.25rem;
    font-size: 2rem;
  }

  .main-card {
    background: #f4faf9;
    border-radius: 10px;
    .country-name {
      text-decoration: underline;
      text-align: center;
      padding: 3rem 0rem;
      font-size: 1.87rem;
    }
    .primary-cards {
      display: flex;
      flex-direction: row;
      flex-wrap: wrap;
      justify-content: center;
      align-items: center;
      padding-bottom: 7rem;

      .secondary-card {
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        padding: 0rem 0.625rem;
        margin: 1.25rem;
        border: 1px solid #000;
        flex-wrap: wrap;
        width: 20%;
        min-width: 20rem;
        max-width: 30rem;
        height: 12.125rem;
        border-radius: 0.625rem;
        box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
        h3 {
          font-size: 1.25rem;
          color: #242058;
          letter-spacing: 0.03em;
        }
        span {
          font-size: 50px;
          letter-spacing: 0.015em;
          color: #7dcea0;
        }
        p {
          letter-spacing: 0.09em;
        }
      }
      .recovered {
        border: 2px solid rgba(39, 174, 96, 0.8);
      }
      .active {
        border: 2px solid rgba(155, 81, 224, 0.8);
        span {
          color: #c396ec;
        }
      }
      .deaths {
        border: 2px solid #fe5050;
        span {
          color: #f86161;
        }
      }
    }
    .search {
      display: flex;
      flex-direction: row;
      justify-content: center;
      padding-bottom: 4rem;
      text-align: center;
      input {
        border: none;
        border-bottom: 3px solid #83c9b5;
      }
    }
  }
}
</style>