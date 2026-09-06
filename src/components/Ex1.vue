<script setup>
import { ref } from 'vue'
const message = ref('Choose your favourite fruit:')
const fruit = ref(['apple', 'orange', 'peach'])
// Add code here
// challenge: use array
</script>

<template>
  <P>{{ message }}</P>

  <label for=""> <input type="radio" name="fruit" /> {{ fruit[0] }} </label>
  <label for=""> <input type="radio" name="fruit" /> {{ fruit[1] }} </label>
  <label for=""><input type="radio" name="fruit" /> {{ fruit[2] }} </label>
</template>

<style scoped></style>
