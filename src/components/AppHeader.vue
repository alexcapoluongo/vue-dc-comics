<template>
    <div class="container">
        <header class="header">
            <div class="logo">
                <img :src="require('/Users/alexcapoluongo/boolean/vue-dc-comics/src/assets/logo.png')" alt="">
            </div>
            <div class="menu">
                <ul 
                class="menu__list">
                    <li
                    v-for="(item, index) in menuList" 
                    :key="index">
                    <a :class="{active : item.active}" href="">{{ item.text }}</a>
                    </li>
                <!-- <li><a class="active" href="">Link</a></li>
                <li><a href="">Link</a></li>
                <li><a href="">Link</a></li>
                <li><a href="">Link</a></li>
                <li><a href="">Link</a></li>
                <li><a href="">Link</a></li>
                <li><a href="">Link</a></li>
                <li><a href="">Link</a></li>
                <li><a href="">Link</a></li>
                <li><a href="">Link</a></li> -->
                </ul>
            </div> 
        </header>
    </div>
</template>

<script>

export default {
    name:"AppHeader",

    data() {
        return {
            menuList: [
                {
                    url: "#",
                    text: "characters",
                    active: false,
                },
                {
                    url: "#",
                    text: "comics",
                    active: true,
                },
                {
                    url: "#",
                    text: "movies",
                    active: false,
                },
                {
                    url: "#",
                    text: "tv",
                    active: false,
                },
                {
                    url: "#",
                    text: "games",
                    active: false,
                },
                {
                    url: "#",
                    text: "collectibles",
                    active: false,
                },
                {
                    url: "#",
                    text: "videos",
                    active: false,
                },
                {
                    url: "#",
                    text: "fans",
                    active: false,
                },
                {
                    url: "#",
                    text: "news",
                    active: false,
                },
                {
                    url: "#",
                    text: "shop",
                    active: false,
                },
            ]
        }
    }
}


</script>

<style lang="scss" scoped>
@import "../style/common.scss";
.header {
    height:15vh;
    min-width:100%;
    background-color: white;
    display: flex;
    justify-content: space-around;
}

.logo {
    width: 10%;
    height:100%;
    display: flex;
    align-items: center;

    img {
        width: 70%;
    }
}

.menu {
    height: 100%;

    &__list {
        list-style: none;
        display: flex;

        li {
            line-height: 15vh;
            padding:5px;
            
            a {
                text-decoration: none;
                font-size: .8em;
                color: #7d818b;
                height: 15vh;
                text-transform: uppercase;

                &.active {
                color: #0082f9;
                border-bottom: 3px solid #0082f9;
                display:flex;
            }

            }
        }
    }

}


</style>