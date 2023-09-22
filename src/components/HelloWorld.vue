<script>
export default {

  name: 'HelloWorld',

  data() {
    return {
      msg: 'Hello Vite!'

    }
  }
}
</script>

<template>
  <h1>{{ msg }}</h1>
</template>

<style lang="scss" scoped>
h1 {
  color: red;

  &:hover {
    color: green;
  }
}
</style>