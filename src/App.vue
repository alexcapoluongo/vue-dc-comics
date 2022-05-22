<template>
  <div id="app">
    <AppHeader/>
    <main>
      <ProductList />
    </main>
    <AppPreFooter/>
    <AppFooter/>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppPreFooter from "./components/AppPreFooter.vue";
import AppFooter from "./components/AppFooter.vue";
import ProductList from "./components/ProductList.vue";

export default {
  components: {
  AppHeader,
  AppPreFooter,
  AppFooter,
  ProductList
  }
}
</script>

<style lang="scss">
@import "./style/common.scss" 
</style>
