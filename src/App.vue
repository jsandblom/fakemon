<script setup lang="ts">
import { ref } from 'vue'

import EKGkurva from './components/EKGkurva.vue'
import EKGsiffra from './components/EKGsiffra.vue'
import saturationKurva from './components/saturationKurva.vue'
import saturationSiffra from './components/saturationSiffra.vue'

const puls = ref(58)

</script>

<template>
  <div>
    <div><EKGkurva :puls="puls" /></div>
    <div><EKGsiffra :puls="puls" /></div>
  </div>
  <div>
    <div><saturationKurva :puls="puls" /></div>
    <div><saturationSiffra :puls="puls" /></div>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
