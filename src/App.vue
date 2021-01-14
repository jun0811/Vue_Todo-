<template>
  <div id="app">
    {{message}}
    <h2> 뒤집힌</h2>
    {{ reverseMessage}}
  </div>
</template>

<script>
export default {
  name: 'App',
  data () {return{
    message : 'hello Vue!'
  }},
  computed: {
    reverseMessage(){
      return this.message.split("").reverse().join("")
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
