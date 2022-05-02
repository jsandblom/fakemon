<script setup lang="ts">
import { reactive, ref } from 'vue'

import EKGkurva from './components/EKGkurva.vue'
import EKGsiffra from './components/EKGsiffra.vue'
import saturationKurva from './components/saturationKurva.vue'
import saturationSiffra from './components/saturationSiffra.vue'

const puls = ref(48)
const sat = ref(59)
const satpuls = reactive({sat: sat.value, puls: puls.value})

</script>

<template>
  <div class="bg-black">
    <div><EKGkurva :puls="puls" /></div>
    <div class="text-blue-600 font-bold"><EKGsiffra :puls="puls" /></div>
    <div><saturationKurva :satpuls="satpuls" /></div>
    <div class="text-green-500 font-bold"><saturationSiffra :satpuls="satpuls" /></div>
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
