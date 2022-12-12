<script>
    export default{
        data(){
            return{
                pages: [
                    "characters", "comics", "movies", "tv", "games", "collectibles", "videos", "fans", "news", "shop" 
                ]
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
        <ul v-for= "element in pages" :key="element" id="nav">
            <li class="nav_item"><a href="">{{element}}</a></li>
        </ul>
    </div>
    
</template>

<style>

</style>