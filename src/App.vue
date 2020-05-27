<template>
  <div id="app">
    <main>
      <div class="search-box">
        <input type="text" class="search-bar" placeholder="search..." />
      </div>

      <div class="weather-wrap">
        <div class="location-box">
          <div class="location">Edmonton, AB</div>
          <div class="date">May 27, 2020</div>
        </div>

        <div class="weather-box">
          <div class="temperature">10°</div>
          <div class="weather">Rain</div>
        </div>
      </div>

    </main>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      api_key: '46e39bae0c6c556b772474591e59dca1'

    }
  }
}
</script>

<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body {
    font-family: 'montserrat', sans-serif;
  }

  #app {
    background-image: url('./assets/cold.jpg');
    background-size: cover;
    background-position: bottom;
    transition: 0.4s;
  }

  main {
    min-height: 100vh;
    padding: 25px;
    background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.25), rgba(0, 0, 0, 0.75));
    }

  .search-box {
    width: 70%;
    margin-bottom: 30px;
    margin-left: 15%;
  }

  .search-box .search-bar {
    width: 100%;
    display: block;
    padding: 15px;
    color: #313131;
    font-size: 20px;

    appearance: none;
    border: none;
    outline: none;
    background: none;
    box-shadow: 0px 0px 8px rgba(0, 0, 0, 0.25);
    background-color: rgba(255, 255, 255, 0.5);
    border-radius: 0px 16px 0px 16px;
    transition: 0.4s;
  }

  .search-box .search-bar:focus {
    box-shadow: 0px 0px 16px rgba(0, 0, 0, 0.25);
    background-color: rgba(255, 255, 255, 0.75);
    border-radius: 16px 0px 16px 0px;
  }


</style>

