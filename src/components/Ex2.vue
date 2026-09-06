<script setup>
import { ref } from 'vue'
const me = ref('/assets/me.png')
const width=ref(400)
const height=ref(300)
let img={ src:me.value, width:width.value, height:height.value }

// Add code here
</script>

<template>
  <!-- Add code here -->
   <!-- sets img value to whatever is inside 'me'-->
   <img v-bind:src="me" v-bind:width="width" v-bind:height="height" alt="me">
   <!--multiple using obj-->
   <img v-bind="img" alt="me">
</template>
