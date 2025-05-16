<template>
  <img :src="imgSrc" v-bind:alt="imgAlt" width="30%">
</template>

<script>
  export default {
    name: 'RandomImagem',
    data(){
      return {
        imgSrc: 'https://wallpapers.com/images/featured/imagens-muito-legais-40it5k0y58kfe71d',
        imgAlt: 'Foto de um planeta'
      }
    }
  }
</script>