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

            <div class="footer__bottom container">
                
                    <div class="footer__bottom__left">
                        <button>SIGN-UP NOW!</button>
                    </div>
                    <div class="footer__bottom__right">
                            
                        <ul>
                            <li><span>FOLLOW US</span></li>
                            <li>
                                <i class="fab fa-facebook"></i>
                            </li>
                            <li>
                                <i class="fab fa-twitter"></i>
                            </li>
                            <li>
                                <i class="fab fa-youtube"></i>
                            </li>
                            <li>
                                <i class="fab fa-pinterest"></i>
                            </li>
                            <li>
                                <i class="fas fa-map-marker-alt"></i>
                            </li>
                        </ul>
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
    background-color: $footer-bar-color;

    &__top {
        height: 40vh;
        background-image: url("/Users/alexcapoluongo/boolean/vue-dc-comics/src/assets/img/footer-bg.jpg");
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

            h3 {
                color: white;
            }

            ul {
                list-style: none;
                margin-bottom:1em;
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
    

        &__left {
            height: 100%;
            width: 50%;
            display: flex;
            align-items:center;

            button {
                padding: 10px;
                border: 2px solid $main-bar-color;
                background-color: $footer-bar-color;
                color: white;
            }
        }

        &__right {
            width: 50%;
            height: 100%;
            display: flex;
            align-items:center;

            ul {
                list-style: none;
                display: flex;
                align-items: center;

                li {
                    margin: 10px;
                    color: white;
                    display: flex;

                    span {
                        color: $main-bar-color;
                    }

                    i {
                        opacity: .5;
                        font-size: 1.5em;
                    }
                }
            }
        }
    }
}

</style>