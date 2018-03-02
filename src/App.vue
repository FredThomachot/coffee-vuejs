<template>
  <div id="app">
    <img src="./assets/logo.png">
    <h1>{{ msg }}</h1>

    <div class="main">
      <toggle-button @change="onChangeEventHandler"/><h2>machine 1</h2><br><br>
      <toggle-button @change="onChangeEventHandler"/><br><br>
      <toggle-button @change="onChangeEventHandler"/><br><br>
    </div>


  </div>
</template>



<script>



export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome Fred'
    }
  }
}

</script>


<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}



h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}

</style>
