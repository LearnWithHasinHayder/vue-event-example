<script setup>
import { ref } from "vue"


function doSomething() {
  console.log("doSomething")
}

</script>

<template>
  <section class="container mx-auto flex items-center flex-col">
    <h1 class="text-center text-2xl py-10">Events Vue.js</h1>
    <form @submit="doSomething()" action="https://google.com/search">
      <input type="text" name="q" />
      <button type="submit" class="ml-5 bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
        Do Something
      </button>
    </form>
  </section>
</template>

<style scoped></style>