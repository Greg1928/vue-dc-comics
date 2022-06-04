<template>
  <footer>
      <div class="footer-top">
          <div class="container">
              <ul>
                  <li><img class="Png" src="../../assets/img/buy-comics-digital-comics.png" alt=""><a href="#">digital comics</a></li>
                  <li><img class="Png" src="../../assets/img/buy-comics-merchandise.png" alt=""><a href="#">dc merchandise</a></li>
                  <li><img class="Png" src="../../assets/img/buy-comics-subscriptions.png" alt=""><a href="#">subscription</a></li>
                  <li><img class="Png" src="../../assets/img/buy-comics-shop-locator.png" alt=""><a href="#">comic shop locator</a></li>
                  <li><img src="../../assets/img/buy-dc-power-visa.svg" alt=""><a href="#">dc power visa</a></li>
              </ul>
          </div>
      </div>
  </footer>
</template>

<script>
export default {
    name: "BaseFooterTop",
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/mixins.scss";

footer{
    z-index: 7;
    .footer-top{
        background-color: var(--primary-color);
        height: 10rem;
        @include InLine;
        align-items: center;
    }
    .container ul{
        @include InLine;
        justify-content: space-between;
        padding: 0 0.5rem;
    }
    li{
        display: flex;
        align-items: center;
        column-gap: .6rem;
    }
    a{
        text-decoration: none;
        color: white;
        font-size: .855rem;
        text-transform: uppercase;
    }
    img{
        height: 2.5rem;
    }
    .Png{
        @include Png;
    }
}


</style>