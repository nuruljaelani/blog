<template>
  <div>
    <nav class="bg-gray-100">
      <div class="flex items-center justify-between mx-auto max-w-6xl py-2 lg:py-3">
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
    <header class="bg-gray-100">
      <div class="flex space-x-4 md:space-x-8 py-4 md:py-10 lg:py-20 justify-center items-center mx-auto max-w-6xl">
        <div class="w-3/5 flex flex-col space-y-4 md:space-y-8">
          <div class="flex">
            <p class="text-xl sm:text-2xl md:text-4xl lg:text-5xl xl:text-6xl font-bold">
              Improve Your&nbsp;
            </p>
            <p class="text-red-500 text-xl sm:text-2xl md:text-4xl lg:text-5xl xl:text-6xl font-bold">
              Skills
            </p>
          </div>
          <p class="text-gray-500">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum distinctio id adipisci minus a reprehenderit, eos illo ipsum dolores quis.
          </p>
          <button type="button" class="bg-red-500 rounded-md py-2 shadow-md block w-32 font-medium text-white">
            Get Started
          </button>
        </div>
        <div class="flex w-2/5">
          <img src="~/assets/Group_94.svg" alt="illustration" class="">
        </div>
      </div>
    </header>
    <main class="mx-auto max-w-6xl my-4 md:my-10 lg:my-16 flex flex-col space-y-4 md:space-y-8">
      <p class="text-lg md:text-xl lg:text-2xl font-semibold">
        New Articles
      </p>
      <div class="flex space-x-4 md:space-x-8">
        <div class="w-1/2 flex flex-col space-y-2">
          <img src="~/assets/images/pankaj-patel-Fi-GJaLRGKc-unsplash.jpg" alt="article images">
          <div class="flex flex-col space-y-2">
            <p class="font-semibold text-lg md:text-xl">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde, delectus.
            </p>
            <p class="text-gray-500">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Animi unde suscipit error cum doloribus est! Ipsam corrupti corporis ipsa consequuntur.
            </p>
          </div>
        </div>
        <div class="w-1/2 flex flex-col space-y-4">
          <div class="flex space-x-4">
            <div class="w-1/2">
              <img src="~/assets/images/fotis-fotopoulos-6sAl6aQ4OWI-unsplash.jpg" alt="article images">
            </div>
            <div class="flex flex-col space-y-4 w-1/2">
              <p class="font-semibold">
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
              </p>
              <p class="text-gray-500 text-sm">
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Minima nulla quas tempora odio impedit sequi perspiciatis dolore culpa ab atque.
              </p>
            </div>
          </div>
          <div class="flex space-x-4">
            <div class="w-1/2">
              <img src="~/assets/images/fotis-fotopoulos-6sAl6aQ4OWI-unsplash.jpg" alt="article images">
            </div>
            <div class="flex flex-col space-y-4 w-1/2">
              <p class="font-semibold">
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
              </p>
              <p class="text-gray-500 text-sm">
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Minima nulla quas tempora odio impedit sequi perspiciatis dolore culpa ab atque.
              </p>
            </div>
          </div>
          <div class="flex space-x-4">
            <div class="w-1/2">
              <img src="~/assets/images/fotis-fotopoulos-6sAl6aQ4OWI-unsplash.jpg" alt="article images">
            </div>
            <div class="flex flex-col space-y-4 w-1/2">
              <p class="font-semibold">
                Lorem ipsum dolor sit amet consectetur adipisicing elit.
              </p>
              <p class="text-gray-500 text-sm">
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Minima nulla quas tempora odio impedit sequi perspiciatis dolore culpa ab atque.
              </p>
            </div>
          </div>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
export default {}
</script>
