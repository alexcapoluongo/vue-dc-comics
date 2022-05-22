<template>
  <div class="product">
    <img :src="productObj.img" alt="" />
    <h4>{{ productObj.title }}</h4>

  </div>
</template>

<script>
export default {
    name: "ProductItem",
    props: {
        productObj: Object,
    }
}
</script>

<style lang="scss" scoped>

.product {
  &__list {
    display: flex;
    flex-wrap: wrap;
  }
}
</style>