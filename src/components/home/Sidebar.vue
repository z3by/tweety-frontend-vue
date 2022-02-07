<template>
  <header role="banner" class="xl:px-3 border-r">
    <div class="sidebar w-[69px] xl:w-64 relative">
      <div class="fixed z-30 top-0 flex flex-col items-center xl:items-start h-screen">
        <div class="tweety-logo flex justify-center">
          <router-link
            to="/home"
            class="hover:bg-sky-100 inline-block rounded-full p-2 w-[50px] h-[50px]"
          >
            <img src="../../assets/img/tweety-logo.svg" alt="Tweety logo" class="w-full" />
          </router-link>
        </div>
        <SidebarNav />
        <div class="flex-1">
          <button class="bg-sky-500 h-13 w-13 xl:w-56 rounded-full text-white my-3">
            <TweetIcon class="inline xl:hidden" />
            <span class="hidden xl:inline font-bold text-lg">Tweet</span>
          </button>
        </div>
        <UserDropDown />
      </div>
    </div>
  </header>
</template>
