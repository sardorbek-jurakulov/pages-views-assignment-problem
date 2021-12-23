<template>
  <div>
    <h1>Products page</h1>
    <nuxt-link to="/" class="link-buttons">Home</nuxt-link>
    <button @click="onLoadDinamicProperties(1, $event)" class="link-buttons">1 - product</button>
    <button @click="onLoadDinamicProperties(2, $event)" class="link-buttons">2 - product</button>
  </div>
</template>

<script>
  export default {
    methods: {
      onLoadDinamicProperties(num, evt) {
        this.$router.push('/products/' + num);
      }
    }
  }
</script>