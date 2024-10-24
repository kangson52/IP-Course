

<!-- <template>
  <header>
    This is my first project
  </header>
</template> -->
<!-- <script setup>
// variable
const msg = 'Hello!'

// functions
function log() {
  console.log(msg)
}
</script>

<template>
  <header>{{ msg }}</header>
</template> -->

<!-- <script src="https://cdn.jsdelivr.net/npm/vue@2/dist/vue.js"></script>

<template>
  <div id="app">{{ message }}</div>
</template>

<script>
  var vue = new Vue({
    el: "#app",
    data: {
      test: "Hello World",
    },
  });

  
</script> -->

<script setup>
import { RouterView } from 'vue-router';
</script>

<template>
  This is my first vuejs project
  <RouterView />
</template>

<style scoped>

</style>
