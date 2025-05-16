<template>
  <div v-if="showName">
    Nome: {{ firstName }}
    <br>
    Sobrenome: {{ lastName }}
  </div>

  <div v-if="acessLevel === 'admin'">Admin</div>
  <div v-else-if="acessLevel === 'marketing'">Marketing</div>
  <div v-else>User</div>
</template>

<script>
  export default {
    name: 'ComponentVIFELSE',
    data() {
      return {
        showHeader: true,
        showName: false,
        firstName: 'Gabriel',
        lastName: 'Zorzi',
        acessLevel: 'admin'
      }
    }
  }
</script>