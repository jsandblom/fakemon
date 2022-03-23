<script setup lang="ts">

const p = defineProps<{puls: number}>()

</script>

<template>
  <div>
    {{ p.puls }}
  </div>
</template>
