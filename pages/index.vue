<template>
  <section>
    <Header />
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
