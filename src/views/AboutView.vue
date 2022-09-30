<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 1.2rem;
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
</style>
