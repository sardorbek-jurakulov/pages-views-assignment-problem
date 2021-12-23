<template>
  <div>
    <h1>Product: № {{ $route.params.pid }}</h1>
    <button @click="loaderHomePage">Home</button>
    <button @click="loaderProductsPage">Products</button>
  </div>
</template>

<script>
  export default {
    methods: {
      loaderHomePage() {
        this.$router.push('/');
      },
      loaderProductsPage() {
        this.$router.push('/products');
      }
    }
  }
</script>