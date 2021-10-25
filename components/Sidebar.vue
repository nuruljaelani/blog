<template>
  <div class="w-1/5">
    <div class="bg-white p-4 flex flex-col">
      <p class="font-bold text-2xl text-red-500 px-8 my-4">
        Admin
      </p>
      <div class="flex flex-col font-medium my-8 px-4">
        <div class="flex flex-col space-y-4">
          <NuxtLink to="/admin" exact>
            <div class="flex items-center space-x-2 rounded-md py-2 px-2">
              <p>Dashboard</p>
            </div>
          </NuxtLink>
          <NuxtLink to="/admin/category">
            <div class="flex items-center space-x-2 py-2 px-2">
              <p>Categories</p>
            </div>
          </NuxtLink>
          <NuxtLink to="/admin/article">
            <div class="flex items-center space-x-2 py-2 px-2">
              <p>Articles</p>
            </div>
          </NuxtLink>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
}
</script>

<style scoped>
.nuxt-link-active {
  background-color: #f87171
}

.nuxt-link-exact-active {
  color: white;
}
</style>
