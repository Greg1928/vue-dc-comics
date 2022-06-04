<template>
  <footer>
      <div class="container">
        <div class="footer-left">
            <div class="left-col">
                <h3>dc comics</h3>
                <ul>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                </ul>
                <h3>dc comics</h3>
                <ul>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                </ul>
            </div>
            <div class="middle-col">
                <h3>dc comics</h3>
                <ul>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                </ul>
            </div>
            <div class="right-col">
                    <h3>dc comics</h3>
                <ul>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                    <li><a href="#">link</a></li>
                </ul>
            </div>
        </div>
        <div class="footer-right"></div>
      </div>
  </footer>
</template>

<script>
export default {
    name: "BaseFooterMiddle",
}
</script>

<style lang="scss" scoped>
@import "../../assets/style/mixins.scss";


footer{
    background-image: url("../../assets/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    height: 22rem;
    

    .container, .footer-left{
        @include InLine;
        justify-content: space-between;
    }
    .footer-left{
        column-gap: 2rem;
        margin-top: 2rem;
    }
    h3{
        color: white;
    }
    .footer-right{
        width: 100%;
        height: 22rem;
        background-position: right;
        background-repeat: no-repeat;
        background-image: url("../../assets/img/dc-logo-bg.png");
    }
    ul{
        margin: 1rem 0;
        list-style: none;
    }
    a{
        text-decoration: none;
        color: var(--tertiary-color);
    }
}

</style>