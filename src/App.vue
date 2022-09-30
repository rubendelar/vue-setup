<script setup>
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "./components/HelloWorld.vue";
import Stadiums from "./components/Stadiums.vue";
</script>

<template>
  <div>
    <nav>
      <RouterLink to="/about">About</RouterLink>
      <RouterLink to="/worldCup">World Cup</RouterLink>
    </nav>

    <Stadiums />

    <RouterView />
  </div>
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
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

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }
  header {
    line-height: 1.5;
    max-height: 100vh;
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
