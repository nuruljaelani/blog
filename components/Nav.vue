<!-- Please remove this file from your project -->
<template>
  <nav class="bg-gray-100">
    <div class="flex items-center justify-between mx-auto max-w-6xl py-2 lg:py-4">
      <NuxtLink to="/">
        <p class="text-lg md:text-xl lg:text-2xl font-bold text-red-500 tracking-tighter">
          My Blog
        </p>
      </NuxtLink>
      <div class="flex space-x-4 md:space-x-8 lg:space-x-12 font-medium">
        <NuxtLink to="/">
          <p class="text-gray-600 hover:text-gray-700">
            Home
          </p>
        </NuxtLink>
        <NuxtLink to="/">
          <p class="text-gray-600 hover:text-gray-700">
            Artikel
          </p>
        </NuxtLink>
        <NuxtLink to="/">
          <p class="text-gray-600 hover:text-gray-700">
            Tutorial
          </p>
        </NuxtLink>
        <NuxtLink to="/login">
          <button type="button" class="bg-red-500 rounded-md text-sm font-medium text-white px-4 py-2">
            Login
          </button>
        </NuxtLink>
      </div>
    </div>
  </nav>
</template>
