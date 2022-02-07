<template>
  <div class="flex">
    <main class="min-w-screen-sm max-w-screen-sm">
      <Navbar title="Home" />
      <TweetInput />
      <Timeline />
    </main>
    <aside class="px-3 py-1 bg-gray-100 hidden lg:(block min-w-64) xl:min-w-80">
      <div>
        <input type="search" placeholder="Search Tweety" class="bg-light-900 mx-auto block w-full rounded-full px-3 py-1" />
      </div>
      <div>
        <h3>Trends for you</h3>
        <h6>Trending in Jordan</h6>
        <ul>
          <li>
            <h4>Topic 1</h4>
          </li>
          <li>
            <h4>Topic 2</h4>
          </li>
          <li>
            <h4>Topic 3</h4>
          </li>
          <li>
            <h4>Topic 4</h4>
          </li>
          <li>
            <h4>Topic 5</h4>
          </li>
        </ul>
      </div>
    </aside>
  </div>
</template>

<route lang="yaml">
meta:
  layout: home
</route>