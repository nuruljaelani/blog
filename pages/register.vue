<template>
  <div>
    <Nav />
    <main class="max-w-6xl mx-auto my-10 md:my-16 lg:my-20" style="min-height:70vh">
      <div class="flex items-center">
        <div class="w-2/3">
          <img src="~/assets/5SCENE.svg" class="w-full">
        </div>
        <div class="w-1/3">
          <div class="bg-white rounded-md shadow-md border p-4 md:p-6 lg:p-8 flex flex-col space-y-4">
            <form class="flex flex-col space-y-4">
              <div class="flex items-center">
                <label class="font-medium w-1/4">
                  Nama Lengkap
                </label>
                <input type="text" class="rounded-md border p-2 w-3/4 appearance-none focus-within:outline-none">
              </div>
              <div class="flex items-center">
                <label class="font-medium w-1/4">
                  Email
                </label>
                <input type="text" class="rounded-md border p-2 w-3/4 appearance-none focus-within:outline-none">
              </div>
              <div class="flex items-center">
                <label class="font-medium w-1/4">
                  Username
                </label>
                <input type="text" class="rounded-md border p-2 w-3/4 appearance-none focus-within:outline-none">
              </div>
              <div class="flex items-center">
                <label class="font-medium w-1/4">
                  Password
                </label>
                <input type="password" class="rounded-md border p-2 w-3/4 appearance-none focus-within:outline-none">
              </div>
              <button type="button" class="bg-red-500 text-white font-medium py-2 rounded-md">
                Register
              </button>
            </form>
            <div class="flex space-x-2">
              <p class="text-gray-500 text-sm">
                Sudah punya akun?
              </p>
              <NuxtLink to="login">
                <p class="text-blue-500 text-sm">
                  Login
                </p>
              </NuxtLink>
            </div>
          </div>
        </div>
      </div>
    </main>
    <Footer />
  </div>
</template>

<script>
import Footer from '../components/Footer.vue'
export default {
  components: { Footer }
}
