<template>
  <div id="app">
    
    <h1>Ralph's Vue Demo</h1>
    <h3>
      Enter text in the box below and it will automatically
      appear below it in upper case.
    </h3>

    <input v-model="data">

    <p class="upper-case-output" v-text="data.toUpperCase()"></p>
    
  </div>
</template>

<script>

export default {
  name: 'app',
  data: function () {
    return {
      data : "Type Something!"
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #1cb3c8;
  margin-top: 60px;
  
}

.upper-case-output {
  border: 2px solid #738598;
  padding: 1.5%;
  margin-left: 25%;
  margin-right: 25%;
  border-radius: 1%;
}

body {
  background-color: #3c415e;
}

</style>
