
<script setup>
  import { ref } from 'vue';
  const count = ref(0);
</script>

<template>
  <main class="container">
    <div class="row text-center justify-content-center mt-5 w-100">
      <h3>the current counter is ...</h3>
      <h1 id="counter-element" class="text-center w-100 display-1 font-weight-bold">
        {{ count }}
      </h1>
      <div class="text-center w-100">
        <button id="minus-button" class="btn btn-warning mx-1" @click="count--">-</button>
        <button id="reset-button" class="btn btn-warning mx-1" @click="count = 0">reset</button>
        <button id="plus-button" class="btn btn-warning mx-1" @click="count++">+</button>
      </div>
    </div>
  </main>
</template>

<style scoped>
main {
  font-family: "Jetbrains mono", sans-serif;
}
</style>
