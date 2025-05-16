<template>
  <header>
    <h1 style="color:red">Header</h1>
    <h3>{{ msg }}</h3>
  </header>
</template>

<script>
  export default {
    name: 'TheHeader',
    props: {
      msg: String
    }
  }
</script>

<style>

</style>