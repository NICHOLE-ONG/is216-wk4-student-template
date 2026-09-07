<script setup>
import { ref } from 'vue'
const me = ref('/assets/me.png')
const width=ref('200')
const height=ref('200') //doesnt matter if got "" ornot bc vue sees it as a string

const img= ref({ src:'/assets/me.png', width:'200', height:'200' })

// Add code here
</script>

<template>
  <!-- Add code here -->
   <!-- sets img value to whatever is inside 'me'-->
   <img v-bind:src="me" v-bind:width="width" v-bind:height="height">
   <!--multiple using obj-->
   <img v-bind="img">
</template>
