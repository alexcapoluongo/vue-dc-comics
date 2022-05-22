<template>
  <section class="products">
    <div class="container">
      <div class="products__list">      
        <ProductItem v-for="(item, index) in products"
        :key="index"
        :productObj="item" />        
      </div>
    </div>
  </section>
</template>

<script>
import ProductItem from "./ProductItem.vue";

export default {
    name: "ProductList",
    components: {
        ProductItem,
    },

    data: function() {
        return {
            products: [
            {
                img: "https://source.unsplash.com/200x200",
                title: "ACTION COMICS"
            },

            {
                img: "https://source.unsplash.com/200x200",
                title: "AMERICAN VAMPIRE 1976"
            },

            {
                img: "https://source.unsplash.com/200x200",
                title: "ACQUAMAN"
            },

            {
                img: "https://source.unsplash.com/200x200",
                title: "BATGIRL"
            },

            {
                img: "https://source.unsplash.com/200x200",
                title: "BATMAN BEYOND"
            },

            {
                img: "https://source.unsplash.com/200x200",
                title: "BATMAN/SUPERMAN"
            },

            {
                img: "https://source.unsplash.com/200x200",
                title: "BATMAN/SUPERMAN ANNUAL"
            },

            {
                img: "https://source.unsplash.com/200x200",
                title: "BATMAN: THE JOKER WAR ZONE"
            },

            {
                img: "https://source.unsplash.com/200x200",
                title: "BATMAN: THREE JOKERS"
            },

            {
                img: "https://source.unsplash.com/200x200",
                title: "BATMAN: THREE JOKERS"
            },

            {
                img: "https://source.unsplash.com/200x200",
                title: "BATMAN: EHITE KNIGHT PRESENTS: HARLEY QUINN"
            },

            {
                img: "https://source.unsplash.com/200x200",
                title: "CATWOMAN"
            },


            ]
        }
    }
}
</script>

<style lang="scss" scoped>

.product {
  width: calc(100% / 6);
}

</style>