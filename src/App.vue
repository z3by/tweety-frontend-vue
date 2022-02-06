<script setup lang="ts">
useHead({
  title: 'Tweety',
  meta: [
    { name: 'description', content: 'A Twitter Clone' },
  ],
})
</script>

<template>
<div class="dark:bg-[#15202B] dark:text-white">
  <router-view />
</div>
</template>
