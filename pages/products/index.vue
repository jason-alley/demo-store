<template>
  <div>
    <div class="grid grid-cols-4 gap-5">
      <div v-for="product in products" :key="product.id">
        <ProductCard :product="product" />
      </div>
    </div>
  </div>
</template>

<script setup>
definePageMeta({
  layout: "products",
});

const { data: products } = await useFetch("https://fakestoreapi.com/products");
useHead({
  title: "Demo Store | Products",
  meta: [
    {
      name: "description",
      content: "This is the products page",
    },
  ],
});
</script>

<style lang="scss" scoped></style>
