 <template>
   <header class="header">
       <div class="header-top"></div>
       <div class="container">
        <div class="header__logo">
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <div class="header__nav">
            <ul>
                <li v-for="(link, i) in links" :key="i" :class="{active : link.current}"><a :href="link.url" @click="current(i)">{{link.text}}</a><div class="bar" :class="{block : link.current}"></div></li>
            </ul>
        </div>
       </div>
   </header>
 </template>
 
 <script>
 export default {
    name: "baseHeader",
    data() {
        return {
            index: 0,
            links: [
                {
                    text: "characters",
                    url: "#",
                    current: false,
                },
                {
                    text: "comics",
                    url: "#",
                    current: false,
                },
                {
                    text: "movies",
                    url: "#",
                    current: false,
                },
                {
                    text: "tv",
                    url: "#",
                    current: false,
                },
                {
                    text: "games",
                    url: "#",
                    current: false,
                },
                {
                    text: "collectibles",
                    url: "#",
                    current: false,
                },
                {
                    text: "videos",
                    url: "#",
                    current: false,
                },
                {
                    text: "fans",
                    url: "#",
                    current: false,
                },
                {
                    text: "news",
                    url: "#",
                    current: false,
                },
                {
                    text: "shops",
                    url: "#",
                    current: false,
                },
                ]
        }
    },
    methods:
    {
        current(i){
            this.index = i;
            for(let i = 0; i<this.links.length; i++){
                if(this.links[i].current === true){
                    this.links[i].current = false;
            }
            }
            this.links[i].current = true;
                
            
            }
            
    },
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
    height: 8.125rem;
    & .header__nav{
        align-self: center;
        margin-top: calc(8.125rem/2);
    } 
    & ul{
        @include InLine;
        column-gap: 1.3rem;
    }
    a{
        text-decoration: none;
        color: black;
        text-transform: uppercase;
        font-size: .8125rem;
        display: flex;
    }
    .active a{
        color: var(--primary-color);
    }
    .bar{
        height: 0.3rem;
        background-color: var(--primary-color);
        display: none;
    }
    li{
        display: flex;
        flex-direction: column;
        height: calc(8.125rem/2);
        justify-content: space-between;
    }
    .header__logo{
        display: flex;
        align-items: center;
    }
    img{
        height: 5.500rem;
    }
    .block{
        display: block;
    }
}

 </style>