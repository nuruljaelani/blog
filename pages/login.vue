<template>
  <div>
    <div class="flex min-h-screen">
      <!-- Sidebar -->
      <sidebar />
    </div>
  </div>
</template>

<script>
import Sidebar from '../../../components/Sidebar.vue'
export default {
  name: 'Category',
  components: Sidebar
}
