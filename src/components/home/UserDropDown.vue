<script setup lang="ts">
const isVisible = ref(false)
</script>

<template>
    <div
        class="flex justify-center xl:justify-start p-2 my-3 h-14 w-14 xl:w-full active:bg-light-900 rounded-full"
        @click="isVisible = !isVisible"
        :class="{ 'bg-light-400': isVisible }"
    >
        <div class="relative w-full">
            <div class="flex justify-center">
                <div class="xl:pr-2">
                    <div class="w-10 rounded-full overflow-hidden">
                        <img
                            src="https://abs.twimg.com/sticky/default_profile_images/default_profile_400x400.png"
                            alt="Profile photo"
                            role="presentation"
                        />
                    </div>
                </div>
                <div class="xl:flex-1 hidden xl:block">
                    <div>
                        <span class="text-sm">User Name</span>
                    </div>
                    <div class="text-cool-gray-500 text-sm">
                        <span>@handle</span>
                    </div>
                </div>
                <div class="hidden xl:flex items-center">
                    <bi-three-dots class />
                </div>
            </div>
        </div>
    </div>
    <div
        class="h-screen w-screen fixed left-0 top-0"
        v-if="isVisible"
        @click="isVisible = !isVisible"
    ></div>
    <div
        class="absolute left-2 xl:left-0 bottom-21 bg-white py-3 rounded-2xl shadow-md w-80 flex flex-col-reverse"
        v-if="isVisible"
    >
        <div class="w-16 overflow-hidden inline-block absolute -bottom-3 left-4">
            <div class="h-3 w-3 bg-white shadow -rotate-45 transform origin-top-left"></div>
        </div>
        <div>
            <div class="flex p-3">
                <div class="pr-2">
                    <div class="w-11 rounded-full overflow-hidden">
                        <img
                            src="https://abs.twimg.com/sticky/default_profile_images/default_profile_400x400.png"
                            alt="Profile photo"
                            role="presentation"
                        />
                    </div>
                </div>
                <div class="flex-1">
                    <div>
                        <span class="text-sm">User Name</span>
                    </div>
                    <div class="text-cool-gray-500 text-sm">
                        <span>@handle</span>
                    </div>
                </div>
                <div class="flex items-center">
                    <bi-check class="text-blue-500 text-2xl" />
                </div>
            </div>
            <div role="separator" class="border-t"></div>
            <div>
                <div class="p-3 text-sm hover:bg-gray-100" role="menuitem">Add an existing account</div>
                <div class="p-3 text-sm hover:bg-gray-100" role="menuitem">Log out @handle</div>
            </div>
        </div>
    </div>
</template>
