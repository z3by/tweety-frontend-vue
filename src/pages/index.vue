<template>
  <div class="welcome h-screen flex flex-col">
    <main class="flex-1">
      <div class="lg:flex lg:flex-1 lg:flex-row-reverse h-full">
        <div class="p-5 lg:mx-10 lg:min-w-xl">
          <div class="tweety-logo">
            <img src="../assets/img/tweety-logo.svg" class="h-16" />
          </div>
          <div>
            <h1 class="text-4xl sm:text-6xl my-9 font-bold">Happening now</h1>
            <h2 class="text-2xl sm:text-4xl font-bold">Join Tweety today.</h2>
            <router-link
              to="/signup"
              class="bg-sky-500 hover:bg-sky-600 py-2 font-bold sm:px-10 rounded-full text-white block sm:w-80 text-center my-3 h-10 max-w-xs"
            >Sign up with phone or email</router-link>
          </div>
          <div class="mt-10">
            <h4 class="mt-5 font-bold">Already have an account?</h4>
            <router-link
              to="/login"
              class="border-gray-300 dark:border-gray-500 border hover:(bg-sky-500 bg-opacity-10) py-2 font-bold sm:px-10 rounded-full text-sky-500 block sm:w-80 text-center my-3 h-10 max-w-xs"
            >Sign in</router-link>
          </div>
        </div>

        <div class="relative flex items-center justify-center">
          <img src="../assets/img/tweety-logo-light.svg" class="absolute w-1/2" />
          <img src="../assets/img/hero-img.png" class="h-full" />
        </div>
      </div>
    </main>

    <footer class="bg-light-400 dark:bg-[#15202B] text-center p-3">
      <nav>
        <a
          href="#"
          v-for="link in navLinks"
          :key="link"
          class="mx-1 text-cool-gray-600 dark:text-cool-gray-400 text-sm hover:underline"
        >{{ link }}</a>
      </nav>
    </footer>
  </div>
</template>

<script setup lang="ts">
const navLinks = [
  "About",
  "Terms of Service",
  "Privacy Policy",
  "Cookie Policy",
  "Help Center",
  "Ads info",
  "Blog",
  "Status",
  "Careers",
  "Brand Resources",
  "Advertising",
  "Marketing",
  "Tweety for Business",
  "Developers",
  "Directory",
  "Settings",
  "© 2021 Tweety, Inc. ",
]
</script>
