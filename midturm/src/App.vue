<template>
  <img alt="Vue logo" src="./assets/me.png" width="200">
  <h1>Name : {{ firstname }} {{ lastname }}</h1>
  <!-- <h1>Name : {{getFullname()}}</h1> -->
  <h1>Age : {{ age }}</h1>
  <h2>Hobby</h2>
  <ul>
    <li>{{ hobby[0]}}</li>
    <li>{{ hobby[1]}}</li>
    <li>{{ hobby[2]}}</li>
  </ul>
  <h2>Basic Information</h2>
  <ul>
    <li>Gender : {{ general.gender }}</li>
    <li>Weight : {{ general.weight }}</li>
    <li>Height : {{ general.height }}</li>
  </ul>
</template>

<script>


export default {
  name: 'App',
  data() {
    return {
      firstname: "Pasin",
      lastname: "Norach",
      age: 20,
      hobby: ["game slot", "Listen to music", "Sleep"],
      general: { gender: "Female", weight: "77", height: 175 }
    }
  },
  methods: {
    getFullname() {
      return this.firstname + this.lastname
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