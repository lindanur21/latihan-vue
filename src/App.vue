<script setup>
import { ref } from 'vue'

const msg = "Hello World"
const rawHtml = "<li>Daftar 1</li>"
const link = "https://www.youtube.com/"
const a = 10
const b = 5
const c = a+b
</script>

<template>
  <div id="app">
      <span>{{ msg }}</span><br>
      <span v-html="rawHtml"></span><br>
      <button :disabled="isButtonDisabled">Button</button><br>
      <span v-bind="objectOfAttrs"></span><br>
      <span style="color: red">Ini harus berwarna merah.</span><br>
      <a v-bind:href="link"> youtube </a><br>
      bil1={{ a }}<br>
      bil2={{ b }}<br>
      hasil={{ c }}


    </div>

</template>
  