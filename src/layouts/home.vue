<template>
  <div class="home flex h-screen justify-center">
    <header
      role="banner"
    >
      <Sidebar />
    </header>
    <main class="flex-1 border-l border-r border-gray-300 dark:border-gray-600
    ">
      <router-view></router-view>
    </main>
  </div>
</template>
