<template>
  <div v-if="brand?.logo">
    <img :src="brand.logo" class="h-full w-full object-cover" />
  </div>
  <img v-else src="/fereloo-logo.png" alt="Fereloo" class="size-8 shrink-0 rounded object-cover" />
</template>

<script setup>
const brand = defineModel({ type: Object, default: () => ({}) })
</script>
