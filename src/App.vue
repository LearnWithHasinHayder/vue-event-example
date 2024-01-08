<script setup>

function doSomething() {
  console.log("you clicked the button")
  // console.log(e.target)
}

function detectKeyPress(e) {
  console.log("you pressed " + e.key)
}

function onlyRunOnEnter() {
  console.log("you pressed enter")
}

function onlyRunOnSpace() {
  console.log("you pressed space")
}

function submitForm() {
  console.log("you submitted the form")
}

</script>

<template>
  <section class="container mx-auto flex items-center flex-col">
    <h1 class="text-center text-2xl py-10">Events Vue.js</h1>
    <form @submit.prevent="submitForm()" action="https://google.com/search">
      <div>
        <!-- <input @keypress.space="onlyRunOnSpace()" @keypress.enter="onlyRunOnEnter()" type="text" name="q" /> -->
        <!-- <button @click="doSomething()" class="ml-5 bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
          Do Something
        </button> -->

        <input type="text" name="q" />
        <button type="submit" class="ml-5 bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
          Submit
        </button>

      </div>
    </form>
  </section>
</template>

<style scoped></style>