<template >
  <div id="Corpo3">
    <button id="spin" v-on:click="Button()">Girar</button>
    <span class="arrow"></span>
    <div id="Inputs">
      <input placeholder="1" v-model="one" type="text">
      <input placeholder="2" v-model="two" type="text">
      <input placeholder="3" v-model="three" type="text">
      <input placeholder="4" v-model="four" type="text">
      <input placeholder="5" v-model="five" type="text">
      <input placeholder="6" v-model="six" type="text">
      <input placeholder="7" v-model="seven" type="text">
      <input placeholder="8" v-model="eight" type="text">
    </div>
    <br>
    <div class="container">
        <div class="one"><h1>{{one}}</h1></div>
        <div class="two"><h1>{{two}}</h1></div>
        <div class="three"><h1>{{three}}</h1></div>
        <div class="four"><h1>{{four}}</h1></div>
        <div class="five"><h1>{{five}}</h1></div>
        <div class="six"><h1>{{six}}</h1></div>
        <div class="seven"><h1>{{seven}}</h1></div>
        <div class="eight"><h1>{{eight}}</h1></div>
    </div>
    <br>
  </div>
</template>
<script>
import { ref } from 'vue'
export default{
  setup() {
    return {
      one: ref(''),
      two: ref(''),
      three: ref(''),
      four: ref(''),
      five: ref(''),
      six: ref(''),
      seven: ref(''),
      eight: ref(''),
    }
  },
  methods:{
    Button(){
      let container = document.querySelector(".container")
let btn = document.getElementById("spin")
let number = Math.ceil(Math.random() * 1000);
    container.style.transform = "rotate(" + number + "deg)";
    number += Math.ceil(Math.random() * 1000);
  }
}
}

</script>
