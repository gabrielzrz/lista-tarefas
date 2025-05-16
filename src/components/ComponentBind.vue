<template>
  <h1 :class="{'title': true, 'title-home': isShowBackGroundColor}">CURSO VUE 3</h1>
</template>

<script>
  export default {
    name: 'ComponentBind',
    data () {
      return {
        isShowBackGroundColor: true
      }
    }
  }
</script>

<style>
  .title{
    font-size: 1.5em;
    color:blue;
  }

  .title-home{
    background-color: black;
  }
</style>