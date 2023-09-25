<script>
export default {

  name: 'AppHeader',

  data() {
    return {
      headerSections: ['CHARACTERS', 'COMICS', 'MOVIES', 'TV', 'GAMES', 'COLLECTIBLES', 'VIDEOS', 'FANS', 'NEWS', 'SHOP'],
    }

  },

}
</script>

<template>
  <nav class="navbar py-0">
    <a class="navbar-brand" href="#">
      <img src="../assets/img/dc-logo.png" alt="DC Logo">
    </a>
    <div id="page" class="d-flex gap-4">
      <a class="py-5" href="##" v-for="section in headerSections">{{ section }}</a>
    </div>
  </nav>
</template>

<style lang="scss" scoped>
@use '../../src/assets/scss/app.scss' as *;

#page {
  a {
    text-decoration: none;
    font-weight: bold;
    color: $dc-secondary;
    border-bottom: 5px solid transparent;
    transition: .5s;

    &:hover {
      color: $dc-primary;
      border-bottom: 5px solid $dc-primary;
    }
  }
}
</style>