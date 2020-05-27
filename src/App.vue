<template>
  <div id="app">
    <main>
      <div class="search-box">
        <input type="text" class="search-bar" placeholder="search..." />
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
  }
</style>

