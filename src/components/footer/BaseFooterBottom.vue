<template>
  <footer>
      <div class="container">
          <div class="footer-left">
              <a href="#">Sign-up Now!</a>
          </div>
          <div class="footer-right">
              <p>follow us</p>
              <img src="../../assets/img/footer-facebook.png" alt="">
              <img src="../../assets/img/footer-twitter.png" alt="">
              <img src="../../assets/img//footer-youtube.png" alt="">
              <img src="../../assets/img/footer-periscope.png" alt="">
              <img src="../../assets/img//footer-pinterest.png" alt="">
          </div>
      </div>
  </footer>
</template>

<script>
export default {
    name: "BaseFooterBottom",
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/mixins.scss";

footer{
    background-color: var(--quaternary-color);

    .container{
        @include InLine;
        justify-content: space-between;
        height: 6.5rem;
    }

    .footer-left{
        align-self: center;
    }
    a{
        text-transform: uppercase;
        color: white;
        text-decoration: none;
        padding: .8125rem 1rem .8125rem 1rem;
        font-size: 1.125rem;
        border: solid var(--primary-color) 2px;
    }

    .footer-right{
        display: flex;
        align-self: center;
        column-gap: 1rem;
    }
    p{
        align-self: center;
        color: var(--primary-color);
        text-transform: uppercase;
        font-weight: bold;
    }
    img{
        cursor: pointer;
    }
}
</style>