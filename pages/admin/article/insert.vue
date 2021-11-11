<template>
  <div>
    <div class="flex min-h-screen">
      <!-- Sidebar -->
      <sidebar />
      <div class="w-4/5 bg-blue-50">
        <div class="flex flex-col space-y-8 py-8 px-8">
          <div class="flex bg-white py-2 shadow justify-end rounded-xl px-4">
            <div class="flex items-center space-x-2">
              <div class="flex bg-gray-200 rounded-full w-10 h-10" />
              <p class="font-medium">
                Admin
              </p>
            </div>
          </div>
          <p class="text-2xl text-blue-600 font-bold">
            Insert Article
          </p>
          <div class="bg-white shadow-md rounded-md">
            <div class="p-4">
              <form class="flex flex-col space-y-6">
                <div class="flex flex-col space-y-2">
                  <label class="text-gray-600 font-medium">
                    Title
                  </label>
                  <input type="text" class="border appearance-none focus:outline-none rounded-md p-2">
                </div>
                <vue-editor v-model="articleContent" />
                <div class="flex text-white font-medium text-sm space-x-4">
                  <button type="button" class="bg-green-500 rounded-lg p-2 shadow font-semibold">
                    Submit
                  </button>
                  <NuxtLink to="/admin/article">
                    <button type="button" class="bg-red-500 rounded-lg p-2 shadow font-semibold">
                      Cancel
                    </button>
                  </NuxtLink>
                </div>
              </form>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Sidebar from '../../../components/Sidebar.vue'

export default {
  components: {
    Sidebar
  },
  data () {
    return {
      articleContent: null
    }
  },
  head: {
    title: 'Insert Article'
  }
}

</script>
