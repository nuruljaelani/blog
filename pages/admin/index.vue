<template>
  <div>
    <div class="flex min-h-screen">
      <div class="w-1/5">
        <div class="bg-white p-4 flex flex-col">
          <p class="font-bold text-2xl text-red-500 px-8 my-4">
            Admin
          </p>
          <div class="flex flex-col font-medium my-8 px-4">
            <div class="flex flex-col space-y-4">
              <div class="flex items-center space-x-2 bg-gray-200 rounded-md py-2 px-2">
                <fa-icon icon="home" />
                <p>Dashboard</p>
              </div>
              <div class="flex items-center space-x-2 py-2 px-2">
                <fa-icon icon="file" />
                <p>Articles</p>
              </div>
              <div class="flex items-center space-x-2 py-2 px-2">
                <fa-icon icon="user" />
                <p>Users</p>
              </div>
            </div>
          </div>
        </div>
      </div>
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
            Dashboard
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
}
</script>
