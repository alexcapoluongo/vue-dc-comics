<template>
  <footer class="footer">
            <div class="footer__top">
                <div class="container">
                    <div class="col-wrap">
                        <div class="footer__top__col">
                            <div class="footer__top__col__up">
                                <h3>DC COMICS</h3>
                                <ul>
                                    <li><a href="">Prova</a></li>
                                    <li><a href="">Prova</a></li>
                                    <li><a href="">Prova</a></li>
                                    <li><a href="">Prova</a></li>
                                    <li><a href="">Prova</a></li>
                                    <li><a href="">Prova</a></li>
                                    <li><a href="">Prova</a></li>
                                </ul>
                            </div>
                            <div class="footer__top__col__down">
                                <h3>SHOP</h3>
                                <ul>
                                    <li><a href="">Prova</a></li>
                                    <li><a href="">Prova</a></li>
                                </ul>
                            
                            </div>
                        </div>
                        <div class="footer__top__col">
                            <h3>DC</h3>
                            <ul>
                                <li><a href="">Prova</a></li>
                                <li><a href="">Prova</a></li>
                                <li><a href="">Prova</a></li>
                                <li><a href="">Prova</a></li>
                                <li><a href="">Prova</a></li>
                                <li><a href="">Prova</a></li>
                                <li><a href="">Prova</a></li>
                                <li><a href="">Prova</a></li>
                                <li><a href="">Prova</a></li>
                                <li><a href="">Prova</a></li>
                                <li><a href="">Prova</a></li>
                                <li><a href="">Prova</a></li>
                            </ul>
                        </div>
                        <div class="footer__top__col">
                            <h3>SITES</h3>
                            <ul>
                                <li><a href="">Prova</a></li>
                                <li><a href="">Prova</a></li>
                                <li><a href="">Prova</a></li>
                                <li><a href="">Prova</a></li>
                                <li><a href="">Prova</a></li>
                            </ul>

                        </div>
                    
                    </div>
                </div>
            </div>

            <div class="footer__bottom">
                <div class="container">
                    <div class="footer__bottom__left">
                        <button>SIGN-UP NOW!</button>
                    </div>
                    <div class="footer__bottom__right">
                        <ul>
                            <li>FOLLOW US</li>
                            <li>F</li>
                            <li>F</li>
                            <li>F</li>
                            <li>F</li>
                            <li>FS</li>
                        </ul>
                    </div>
                </div>
            </div>
      
  </footer>
</template>

<script>
export default {
    name:"AppFooter",
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";
@import "../style/variables.scss";

.footer {
    height:50vh;
    background-color: green;

    &__top {
        height: 40vh;
        background-image: url("/Users/alexcapoluongo/boolean/vue-dc-comics/img/footer-bg.jpg");
        display: flex;
        justify-content: flex-start;


        .col-wrap {
            height: 100%;
            width: 400px;
            display:flex;
        }

        &__col {
            width: calc(100% / 3);
            height:100%;
            border: 2px solid red;

            h3 {
                color: white;
            }

            ul {
                list-style: none;
                li {
                    a{
                        text-decoration: none;
                        color: #505661;
                    }
                }  
            }
        }
    }

    &__bottom {
        height: 10vh;
        background-color: $footer-bar-color;
        display: flex;
        justify-content: space-around;
        align-items: center;

        &__left {
            height: 100%;
            width: 20%;
            button {
                padding: 5px;
                border: 2px solid $main-bar-color;
                background-color: $footer-bar-color;
                color: white;
            }
        }

        &__right {
            width: 80%;
            height: 100%;
        }
    }
}

</style>