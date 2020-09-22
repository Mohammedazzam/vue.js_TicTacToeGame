<template>
  <div id="app">
    <h1>Tic-Tac-Toe Game</h1>
    <Grid />
  </div>
</template>

<script>
import Grid from './components/Grid'
export default {
  name: "App",
  components: {
    Grid
  },
  data () {
    return {
      matches:0,
      wins:{
        O:0,
        X:0
      }
    }
  }
};
</script>

<style>

#app {
  font-family: 'Dosis', sans-serif;
  text-align: center;
  color: #2c3e50;
  margin: 0 auto;
  max-width: 400px;
}

#app h1{
  text-transform: uppercase;
  font-weight: bold;
  font-size: 3em;
}


</style>
