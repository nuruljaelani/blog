<template>
  <div>
    <Nav />
    <main class="mx-auto max-w-6xl my-4 md:my-10 lg:my-16 min-h-screen">
      <div class="flex space-x-4 md:space-x-8 my-4 md:my-8">
        <div class="w-3/4 flex flex-col space-y-4">
          <p class="text-xl md:text-2xl lg:text-3xl font-semibold">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Facilis doloremque consectetur ab eveniet
          </p>
          <hr>
          <img src="~/assets/images/pankaj-patel-Fi-GJaLRGKc-unsplash.jpg" alt="article images">
          <p class="font-normal antialiased tracking-wide leading-loose">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Eos sunt dolores consequuntur eaque. At a dolores omnis saepe suscipit excepturi illo quidem vero, quam ab quisquam velit. Quaerat similique quod voluptatibus nisi a neque placeat id quam itaque incidunt beatae architecto obcaecati nam ullam, vero maxime inventore hic recusandae est, tempora tempore labore. Quia vel ad provident voluptatibus obcaecati ullam repellat nihil? Possimus totam saepe dicta nesciunt fugiat. Earum eum aperiam veniam delectus corrupti quae quibusdam similique, cumque debitis, laudantium accusamus perferendis rerum sequi unde saepe cupiditate sit assumenda. Amet, nulla? Culpa, obcaecati ab consequuntur maiores, fuga, neque voluptates repellat magni labore nobis quis corporis aut perspiciatis. Magnam omnis hic dicta earum, odit officia voluptate ad harum laudantium ea sint? Esse nam similique ex voluptatum non dignissimos voluptates harum modi cum in porro, fuga delectus, animi consequuntur dolorum qui maxime dolorem ratione tenetur minus quibusdam nihil? Similique eaque sequi corporis autem dolor deleniti inventore nulla ullam maxime illo illum tenetur tempora repellendus aspernatur magnam voluptates ipsum nesciunt, iste optio assumenda harum nihil totam ab? Nobis, mollitia. Nemo soluta totam non placeat, eos magnam, eligendi nam atque nostrum temporibus ea unde facere libero veritatis exercitationem saepe laudantium, accusamus iste est repellendus.
          </p>
        </div>
        <div class="w-1/4 border h-full p-2">
          <p class="font-semibold text-lg md:text-xl">
            Categories
          </p>
          <div class="flex flex-col font-medium my-4 space-y-2 text-gray-500">
            <p>
              #&nbsp;&nbsp;Php
            </p>
            <p>
              #&nbsp;&nbsp;Javascript
            </p>
            <p>
              #&nbsp;&nbsp;Phyton
            </p>
            <p>
              #&nbsp;&nbsp;Golang
            </p>
            <p>
              #&nbsp;&nbsp;Laravel
            </p>
          </div>
        </div>
      </div>
      <hr>
      <div class="flex flex-col my-4 lg:my-10 lg:my-16 space-y-8">
        <p class="text-xl md:text-2xl lg:text-3xl font-medium">
          Tutorial lainya
        </p>
        <div class="grid grid-cols-1 md:grid-cols-4 gap-4">
          <div class="flex flex-col space-y-2 bg-gray-50 border">
            <img src="~/assets/images/fotis-fotopoulos-6sAl6aQ4OWI-unsplash.jpg" alt="article images">
            <div class="flex flex-col p-4">
              <p class="text-red-500 font-medium text-sm">
                javascript
              </p>
              <p class="font-medium">
                Lorem ipsum dolor, sit amet consectetur
              </p>
            </div>
          </div>
          <div class="flex flex-col space-y-2 bg-gray-50 border">
            <img src="~/assets/images/fotis-fotopoulos-6sAl6aQ4OWI-unsplash.jpg" alt="article images">
            <div class="flex flex-col p-4">
              <p class="text-red-500 font-medium text-sm">
                javascript
              </p>
              <p class="font-medium">
                Lorem ipsum dolor, sit amet consectetur
              </p>
            </div>
          </div>
          <div class="flex flex-col space-y-2 bg-gray-50 border">
            <img src="~/assets/images/fotis-fotopoulos-6sAl6aQ4OWI-unsplash.jpg" alt="article images">
            <div class="flex flex-col p-4">
              <p class="text-red-500 font-medium text-sm">
                javascript
              </p>
              <p class="font-medium">
                Lorem ipsum dolor, sit amet consectetur
              </p>
            </div>
          </div>
          <div class="flex flex-col space-y-2 bg-gray-50 border">
            <img src="~/assets/images/fotis-fotopoulos-6sAl6aQ4OWI-unsplash.jpg" alt="article images">
            <div class="flex flex-col p-4">
              <p class="text-red-500 font-medium text-sm">
                javascript
              </p>
              <p class="font-medium">
                Lorem ipsum dolor, sit amet consectetur
              </p>
            </div>
          </div>
        </div>
      </div>
    </main>
    <footer class="bg-gray-100">
      <div class="flex justify-between max-w-6xl py-4 md:py-8 lg:py-12 mx-auto">
        <p class="text-sm text-gray-500">
          &copy;&nbsp;2021 goblog.com
        </p>
        <div class="flex space-x-3">
          <img src="~/assets/logo/github-icon.svg" alt="" class="w-6">
          <img src="~/assets/logo/instagram-icon.svg" alt="" class="w-6">
          <img src="~/assets/logo/facebook.svg" alt="" class="w-6">
          <img src="~/assets/logo/youtube-icon.svg" alt="" class="w-6">
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
import Nav from '~/components/Nav'

export default {
  components: {
    Nav
  }
}
</script>
