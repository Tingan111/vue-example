<script setup>
import {ref}from 'vue'; 
const message=ref('Hello world')

function ReverseMessage(){
  message.value=message.value.split('').reverse().join('')
}
</script>
<template>
  <h1>{{ message }}</h1>
  <button @click="ReverseMessage">Reverse Message</button>
  <button @click="message+='!'">append"!"</button>
  <a href="https://vuejs.org" @click.prevent="notify">
    A link with e.preventDefault()
  </a>
</template>
<style>
button, a{


}
</style>