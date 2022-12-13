<script>
    export default{
        data(){
            return{
                pages: [
                    {text: "characters",
                    url: "#",
                    current: false},
                    {text: "comics", 
                    url: '#',
                    current: false},
                    {text: "movies",
                    url: '#',
                    current: false},
                    {text: "tv",
                    url: '#',
                    current: false},
                    {text: "games", 
                    url: '#',
                    current: false},
                    {text: "collectibles",
                    url: '#',
                    current: false},
                    {text: "videos",
                    url: '#',
                    current: false}, 
                    {text: "fans",
                    url: '#',
                    current: false},
                    {text: "news",
                    url: '#',
                    current: false}, 
                    {text: "shop",
                    url: '#',
                    current: false} 
                ],
            }
        },
        methods: {

        }
    }
</script>

<template>
    <div id="header">
        <a href="#" id="logo">
            <img src= "../../assets/img/dc-logo.png" alt="">
        </a>
        <ul id="nav">
            <li v-for= "(element, index) in pages" :key="index" class="nav_item"><a href="element.url">{{element.text}}</a></li>
        </ul>
    </div>   
</template>

<style lang="scss">
    @use "../../assets/scss/variables.scss";

    #header{
        min-width:1280px;
        height:80px;
        background-color:#fff;
        padding:0;
        @include flex_row_around;

            #logo{
                flex-basis: 10%;
                    img{
                        width: 50px;
                        height: 50px;
                    }
            }

            #nav{
                flex-basis: 70%;
                @include flex_row_around;

                    .nav_item{
                        list-style: none;
                            a{
                                text-transform: uppercase;
                            }
                    }
            }
    }
</style>