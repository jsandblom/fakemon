<script setup lang="ts">
import { ref } from 'vue'

const p = defineProps<{puls: number}>()
</script>

<template>
  <div>
    {{ p.puls }}
  </div>
</template>

