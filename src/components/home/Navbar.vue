<script setup lang="ts">
defineProps<{ title: string }>()
</script>

<template>
  <div class="navbar p-3">
    <h1>{{ title }}</h1>
  </div>
</template>
