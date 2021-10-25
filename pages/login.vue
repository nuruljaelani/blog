<template>
  <div>
    <Nav />
    <main class="max-w-6xl mx-auto my-10 md:my-16 lg:my-20" style="min-height:70vh">
      <div class="flex items-center">
        <div class="w-3/5">
          <img src="~/assets/9SCENE.svg" class="w-full">
        </div>
        <div class="w-2/5">
          <div class="bg-white rounded-md shadow-md border p-4 md:p-6 lg:p-8 flex flex-col space-y-4">
            <form class="flex flex-col space-y-4">
              <div class="flex items-center">
                <label class="font-medium w-1/4">
                  Username
                </label>
                <input type="text" class="rounded-md border p-2 w-3/4 appearance-none focus-within:outline-none">
              </div>
              <div class="flex flex-col space-y-1">
                <p class="text-xs text-gray-400 flex justify-end">
                  Lupa Password?
                </p>
                <div class="flex items-center">
                  <label class="font-medium w-1/4">
                    Password
                  </label>
                  <input type="password" class="rounded-md border p-2 w-3/4 appearance-none focus-within:outline-none">
                </div>
              </div>
              <button type="button" class="bg-red-500 text-white font-medium py-2 rounded-md">
                Login
              </button>
            </form>
            <div class="flex space-x-2">
              <p class="text-gray-500 text-sm">
                Belum punya akun?
              </p>
              <NuxtLink to="/register">
                <p class="text-blue-500 text-sm">
                  Daftar
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
  components: { Footer },
  head: {
    title: 'Login'
  }
}
