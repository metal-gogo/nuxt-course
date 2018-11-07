<template>
  <section class="container">
    <nuxt-link to="/users">Users</nuxt-link>
    <button @click="onLoadProducts">Products</button>
  </section>
</template>

<script>
export default {
  methods: {
    onLoadProducts() {
      this.$router.push('/products');
    },
  },
};
</script>


<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
