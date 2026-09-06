<script setup>
import { ref } from 'vue'
const option = ref('Username login') //default it first
// Add code here
</script>

<template>
  <h1>Please select your login option</h1>
  <!-- Add/modify code in the following to have a dropdown list 
        which lets the user to select either to login with username or email -->
  <select v-model="option">
    <option selected>Username login</option>
    <option>Email login</option>
  </select>
  <div v-if="option=='Username login'"> 
    <label>Username</label>
    <input placeholder="Enter your username" />
</div>
  <div v-else>
    <label>Email</label>
    <input placeholder="Enter your email address" />
</div>

</template>
