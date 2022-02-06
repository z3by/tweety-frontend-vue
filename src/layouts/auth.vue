<template>
    <main class="h-screen bg-gray-400 dark:bg-gray-600 flex justify-center items-center">
        <div
            class="modal h-screen md:h-screen-sm w-screen md:w-xl bg-white dark:bg-[#15202B] mx-auto rounded-2xl"
        >
            <div class="modal-header p-2 flex">
                <router-link
                    to="/"
                    class="h-10 w-10 hover:bg-light-600 active:bg-gray-300 text-2xl rounded-full flex items-center justify-center"
                >
                    <bi-x />
                </router-link>
                <div class="flex justify-center flex-1">
                    <img src="../assets/img/tweety-logo.svg" alt="Tweety logo" class="h-10 w-10" />
                </div>
            </div>
            <div class="modal-body py-6 px-8 font-bold">
                <router-view></router-view>
            </div>
        </div>
    </main>
</template>
