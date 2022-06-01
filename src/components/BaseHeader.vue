 <template>
   <header class="header">
       <div class="header-top"></div>
       <div class="container">
        <div class="header__logo">
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <div class="header__nav">
            <ul>
                <li><a href="#">link</a></li>
                <li class="active"><a href="#">link</a></li>
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
       </div>
   </header>
 </template>
 
 <script>
 export default {
    name: "baseHeader",
 }
 </script>
 
 <style lang="scss" scoped>
@import "../assets/style/mixins.scss";

.header-top{
    background-color: var(--secondary-color);
    height: 2.5rem;
}

.container{
    @include InLine;
    justify-content: space-between;
    padding: 1rem 0;

    & .header__nav{
        align-self: center;
    } 
    & ul{
        @include InLine;
        column-gap: 1rem;
    }
    a{
        padding: 1rem;
        text-decoration: none;
        color: black;
    }
    .active a{
        color: var(--primary-color);
    }
}

 </style>