<template>
  <div>
    <h1>{{ stadium }}</h1>
    <br />
    <img
      src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRSrK6BYxYpjDYUNzSrx9ZRtCB7Vzjj5b9aig&usqp=CAU"
      alt="Cruces mundial 2022"
    />
    <br />

    <button @click="worldCup">Click to see World Cup Dates!</button>
  </div>
</template>

<script setup>
import { ref } from "vue";
const stadium = ref("World cup final will be placed in Qatar this winter");

function worldCup() {
  console.log("World Cup in winter time, LoL.....");
  alert("World Cup in winter time, LoL.....");
}
</script>

<style>
div {
  display: flex;
  justify-content: center;
  flex-direction: column;
}
h1 {
  font-weight: 700;
  font-size: 1.3rem;
  top: -10px;
  text-align: center;
}
h2 {
  font-size: 2rem;
  font-weight: bold;
}
@media (min-width: 1024px) {
  div {
    min-height: 150px;
    display: flex;
    align-items: center;
    flex-direction: column;
    margin-top: 1px;
  }
}
img {
  width: 80%;
  align-self: center;
}
button {
  width: 40%;
  padding: 0.5rem 1rem;
  border-radius: 10px;
  align-self: center;
  background-color: mediumblue;
  color: white;
  font-size: 20px;
}
</style>
