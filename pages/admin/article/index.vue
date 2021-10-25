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
            Article
          </p>
          <NuxtLink to="/admin/article/insert">
            <button type="button" class="bg-orange-500 rounded-md p-2 text-white text-sm font-medium w-32 shadow hover:bg-orange-600">
              Add Article
            </button>
          </NuxtLink>
          <div class="bg-white shadow-md rounded-md">
            <table class="mx-auto w-full p-4">
              <thead class="font-medium bg-gray-100 w-full p-4">
                <tr>
                  <td class="p-4">
                    No
                  </td>
                  <td class="p-4">
                    Title
                  </td>
                  <td class="p-4">
                    Description
                  </td>
                  <td class="p-4">
                    Category
                  </td>
                  <td class="p-4">
                    Action
                  </td>
                </tr>
              </thead>
              <tbody v-for="(post, index) in posts" :key="index">
                <tr>
                  <td class="p-4">
                    {{ index + 1 }}
                  </td>
                  <td class="p-4">
                    {{ post.title }}
                  </td>
                  <td class="p-4">
                    {{ post.body }}
                  </td>
                  <td class="p-4">
                    Javascript
                  </td>
                  <td class="p-4">
                    <button type="button" class="bg-blue-500 rounded text-xs p-1 text-white">
                      Edit
                    </button>
                  </td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Sidebar from '../../../components/Sidebar.vue'
export default {
  name: 'Article',
  components: Sidebar,
  async asyncData ({ $axios }) {
    const posts = await $axios.$get('https://jsonplaceholder.typicode.com/posts')
    return { posts }
  },
  head: {
    title: 'Data Article'
  }
}

</script>
