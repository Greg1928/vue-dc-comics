<template>
  <footer>
      <div class="footer-top">
          <div class="container">
              <ul>
                  <li><img class="Png" src="../../assets/img/buy-comics-digital-comics.png" alt=""><a href="#">link</a></li>
                  <li><img class="Png" src="../../assets/img/buy-comics-merchandise.png" alt=""><a href="#">link</a></li>
                  <li><img class="Png" src="../../assets/img/buy-comics-subscriptions.png" alt=""><a href="#">link</a></li>
                  <li><img class="Png" src="../../assets/img/buy-comics-shop-locator.png" alt=""><a href="#">link</a></li>
                  <li><img src="../../assets/img/buy-dc-power-visa.svg" alt=""><a href="#">link</a></li>
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
    .footer-top{
        background-color: var(--primary-color);
        height: 10rem;
        @include InLine;
        align-items: center;
    }
    .container ul{
        @include InLine;
        justify-content: space-around;
    }
    li{
        display: flex;
        align-items: center;
        column-gap: 1rem;
    }
    a{
        text-decoration: none;
        color: white;
        font-size: 1.25rem;
    }
    img{
        height: 2.5rem;
    }
    .Png{
        @include Png;
    }
}


</style>