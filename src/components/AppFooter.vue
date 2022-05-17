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
                        </div>
                        <div class="footer__top__col">
                            <h3>SITES</h3>
                            <li><a href="">Prova</a></li>
                            <li><a href="">Prova</a></li>
                            <li><a href="">Prova</a></li>
                            <li><a href="">Prova</a></li>
                            <li><a href="">Prova</a></li>

                        </div>
                    
                    </div>
                </div>
            </div>

            <div class="footer__bottom"></div>
      
  </footer>
</template>

<script>
export default {
    name:"AppFooter",
}
</script>

<style lang="scss" scoped>
@import "../style/common.scss";

.footer {
    height:50vh;
    background-color: green;

    &__top {
        height: 40vh;
        background-color: black;
        display: flex;
        justify-content: flex-start;

        ul {
                
                list-style: none;

                li {

                    a {
                        text-decoration: none;
                        color:black
                    }
                }
            }

        .col-wrap {
            height: 100%;
            width: 400px;
            background-color: aquamarine;
            display:flex;
        }

        &__col {
            width: calc(100% / 3);
            height:100%;
            border: 2px solid red;
        }
    }

    &__bottom {
        height: 10vh;
        background-color: green;
    }
}

</style>