<template>
    <section class="prefooter">
        <div class="container">
            <ul class="icons-list">
                <li 
                v-for="(item, index) in icons" 
                :key="index" >
                    <img 
                    :src="require(`../assets/img/${ item.img }`)">
                    <h3> {{ item.text }} </h3>
                </li>
            </ul>
        </div>
    </section>
</template>

<script>
export default {
    name: "AppPreFooter",
    data: function() {
        return {
            icons: [
                {
                    img: 'buy-comics-digital-comics.png',
                    text: 'Digital Comics'
                },

                {
                    img: 'buy-comics-merchandise.png',
                    text: 'DC Merchandise'
                },

                {
                    img: 'buy-comics-subscriptions.png',
                    text: 'Subscription'
                },

                {
                    img: 'buy-comics-shop-locator.png',
                    text: 'Comic shop locator'
                },


                {
                    img: 'buy-dc-power-visa.svg',
                    text: 'DC power visa'
                },

            ]
        }
    }
}

</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.prefooter {
    background-color: $main-bar-color;
    color: white;

    .icons-list {
        display: flex;

        li {
            width: calc(100% / 4);
            display: flex;

            img {
                width: 40%;
                height: 70%;
                margin-right: 1rem;
                padding: 1rem;
            }

            
        }
    }
}
</style>