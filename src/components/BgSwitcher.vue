<template>
  <div class="flex gap-1">
    <div v-for="color in colors" :key="color" class="flex flex-col items-center"
         :class="`bg-${color} w-16 h-16 rounded-lg`">
    </div>
  </div>
</template>

<script setup lang="ts">
const colors = ['base-100', 'base-200', 'base-300', 'base-400', 'base-500', 'base-600', 'base-700', 'base-800', 'base-900']

</script>

<style scoped>

</style>