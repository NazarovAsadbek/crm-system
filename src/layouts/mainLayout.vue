<template>
  <div class="app-main-layout">
    <navbar />
    <sidebar />

    <main class="app-content">
      <div class="app-page">
        <router-view />
      </div>
    </main>

    <div class="fixed-action-btn">
      <a class="btn-floating btn-large blue" href="#">
        <i class="large material-icons">add</i>
      </a>
    </div>
  </div>
</template>
<script>
import navbar from '@/components/app/Navbar'
import sidebar from '@/components/app/Sidebar'

export default {
  components: {
    navbar, sidebar
  },
  data: () => ({

  })
}
</script>
