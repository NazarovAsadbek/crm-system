<template>
  <ul class="sidenav app-sidenav open" >
    <router-link v-for="(link, id) in links" :key="id" tag="li" active-class="active" exact :to="link.to">
      <a class="waves-effect waves-orange pointer">{{ link.title }}</a>
    </router-link>
  </ul>
</template>

<script>
export default {
  data: () => ({
    links: [
      {title: 'Счёт', to: '/'},
      {title: 'История', to: '/history'},
      {title: 'Планирование', to: '/planning'},
      {title: 'Новая запись', to: '/record'},
      {title: 'Категория', to: '/categories'},
    ]
  }),
}
</script>

<style lang="scss" scoped>

</style>
