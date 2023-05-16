<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <header>
    <div class="container justify-center mx-auto px-20 py-10">
      <nav>

        <ul
          class="hidden text-sm font-medium text-center text-gray-500 divide-x divide-gray-200 rounded-lg shadow sm:flex dark:divide-gray-700 dark:text-gray-400">
          <li class="w-full">
            <RouterLink to="/"
              class="inline-block w-full p-4 text-gray-500 bg-white hover:text-gray-700 hover:bg-gray-50 rounded-l-lg focus:ring-4 focus:ring-blue-300 focus:outline-none dark:bg-gray-700 dark:text-white"
              >Home</RouterLink>
          </li>  
          <li class="w-full">
            <RouterLink to="/aplikasiku"
              class="inline-block w-full p-4 bg-white rounded-r-lg hover:text-gray-700 hover:bg-gray-50 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:hover:text-white dark:bg-gray-800 dark:hover:bg-gray-700">Aplikasiku
            </RouterLink>
          </li>
        </ul>
      </nav>
    </div>



    <div>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
nav a.router-link-exact-active {
  @apply text-blue-500;
}
</style>
