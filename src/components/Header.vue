<script>
export default {

  name: 'Header',

  data() {
    return {
      headerSections: ['CHARACTERS', 'COMICS', 'MOVIES', 'TV', 'GAMES', 'COLLECTIBLES', 'VIDEOS', 'FANS', 'NEWS', 'SHOP'],
    }
  }
}
</script>

<template>
  <nav class="navbar">
    <div class="container">
      <a class="navbar-brand" href="#">
        <img src="../assets/img/dc-logo.png" alt="DC Logo">
      </a>
      <div class="d-flex gap-4">
        <a href="##" v-for="section in headerSections">{{ section }}</a>
      </div>
    </div>
  </nav>
</template>

<style lang="scss" scoped></style>