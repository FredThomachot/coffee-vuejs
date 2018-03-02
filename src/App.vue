
<template>
  <div id="app">
    <img src="./assets/logo.png">
    <h1>{{ msg }}</h1>
    <ul>
      <li>
        <div class="buttons" v-for="machine in machines">
          <label v-bind:class="{ bold: machine.state }" for="name">Machine {{machine.id}} </label><toggle-button v-model="machine.state"/>
        </div>

      </li>
    </ul>

  </div>

</template>

<script>



export default {
  name: 'app',
  data () {
    return {
      msg: 'My coffee machines',
      machines: [
        {id:1, state:true},
        {id:2, state:true},
        {id:3, state:true},
        {id:4, state:true},
        {id:5, state:true}
      ]
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

.bold{
  font-weight: bold;
}


.buttons {
  margin-bottom: 30px;
  margin-top: 30px;
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
