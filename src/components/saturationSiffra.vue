<script setup lang="ts">

interface SatPuls {
  puls: number,
  sat: number
}

const p = defineProps<{satpuls: SatPuls}>()

</script>

<template>
  <div>
    <span>{{ p.satpuls.puls }}</span>
    <span>{{ p.satpuls.sat }}</span>
  </div>
</template>
