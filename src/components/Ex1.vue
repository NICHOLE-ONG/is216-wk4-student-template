<script setup>
import { ref } from 'vue'
const message = ref('Choose your favorite fruit:')
const fruit = ref(['apple', 'orange', 'peach'])
// Add code here
// challenge: use array
</script>

<template>
  {{ message }}

  <label for=""> <input type="radio" name="fruit" /> {{ fruit[0] }} </label>
  <label for=""> <input type="radio" name="fruit" /> {{ fruit[1] }} </label>
  <label for=""><input type="radio" name="fruit" /> {{ fruit[2] }} </label>
  <!--can also use for loop-->
<!--<label v-for="fruit in fruits" :key="fruit"> <input type="radio" name="fruit"> {{fruit}} </label>-->
</template>

<style scoped></style>
