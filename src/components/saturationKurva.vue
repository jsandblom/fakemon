<script setup lang="ts">

interface SatPuls {
  puls: number,
  sat: number
}

const props = defineProps<{satpuls: SatPuls}>()

</script>

<template>
  <div>
    <span>[{{ props.satpuls.sat }}]</span>
  </div>
</template>
