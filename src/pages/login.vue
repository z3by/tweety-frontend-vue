<template>
  <div>
    <h3 class="text-2xl">Sign in to Tweety</h3>
    <form>
      <Input v-model="userId" name="Phone, email or user name" type="text" />
      <Input v-model="password" name="Password" type="password" />
      <Button class="w-full mt-5" :disabled="false">Log in</Button>
    </form>
    <p class="font-normal my-8 block text-cool-gray-600">
      Don't have an account?
      <router-link to="/signup" class="text-sky-600">Sign up</router-link>
    </p>
  </div>
</template>

<script lang="ts" setup>
import { ref } from "@vue/reactivity";

const userId = ref<string>("");
const password = ref<string>("");
</script>

<route lang="yaml">
meta:
  layout: auth
</route>
