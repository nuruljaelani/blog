<template>
  <div>
    <nav class="bg-gray-50">
      <div class="flex items-center justify-between mx-auto max-w-7xl py-2 lg:py-3">
        <p class="text-lg md:text-xl lg:text-2xl font-bold text-red-500 tracking-tighter">
          Go Blog
        </p>
        <div class="flex space-x-4 md:space-x-8 lg:space-x-12 font-medium">
          <p>Home</p>
          <p>Article</p>
          <p>Tutorial</p>
          <p>About</p>
        </div>
      </div>
    </nav>
    <header class="bg-gray-50">
      <div class="flex py-4 md:py-10 lg:py-20 justify-center items-center mx-auto max-w-7xl">
        <div class="w-1/2 flex flex-col space-y-4 md:space-y-8">
          <div class="flex">
            <p class="text-xl sm:text-2xl md:text-4xl lg:text-5xl xl:text-6xl font-bold">
              Improve Your&nbsp;
            </p>
            <p class="text-red-500 text-xl sm:text-2xl md:text-4xl lg:text-5xl xl:text-6xl font-bold">
              Skills
            </p>
          </div>
          <button type="button" class="bg-red-500 rounded-md py-2 shadow-md block w-32 font-medium text-white">
            Get Started
          </button>
        </div>
        <div class="flex w-1/2">
          <img src="~/assets/Group_94.svg" alt="illustration" class="px-8 md:px-20">
        </div>
      </div>
    </header>
  </div>
</template>

<script>
export default {}
</script>
