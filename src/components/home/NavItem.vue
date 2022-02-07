<script setup lang="ts">
const props = defineProps<{ text: string; to?: string }>()

const route = useRoute();
const isActive = computed(() => route.path.toString() === props.to);
</script>

<template>
    <li class="py-1 flex justify-center xl:justify-start">
        <component
            :is="to ? 'router-link' : 'div'"
            :to="to"
            class="p-3 inline-block hover:bg-gray-200 focus:bg-gray-300 cursor-pointer rounded-full"
        >
            <div class="flex">
                <slot name="prefix" :active="isActive"></slot>
                <span
                    class="hidden xl:inline text-xl ml-5 mr-4 font-normal"
                    :class="{ '!font-bold': isActive }"
                >{{ text }}</span>
            </div>
        </component>
    </li>
</template>
