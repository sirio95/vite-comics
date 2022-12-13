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

<style>

</style>