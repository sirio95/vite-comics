<script>

export default{
    data(){
        return{
            social_icons: [
                {
                    name: 'facebook',
                    src: 'footer-facebook.png',
                    url: '#'
                },
                {
                    name: 'twitter',
                    src: 'footer-twitter.png',
                    url: '#'
                },
                {
                    name: 'youtube',
                    src: 'footer-youtube.png',
                    url: '#'
                },
                {
                    name: 'pinterest',
                    src: 'footer-pinterest.png',
                    url: '#'
                },
                {
                    name: 'periscope',
                    src: 'footer-periscope.png',
                    url: '#'
                }
            ]
        }
    },
    methods: {
        getImageByURL(name){
            return new URL(`../../assets/img/${name}`, import.meta.url).href;
        }
    }
    
}
</script>

<template>
    <div>
        <div id="sign">
            <a href="">SIGN-UP NOW!</a>
        </div>
        <div id="social">
            <h3>FOLLOW US</h3>
            <ul id="icons">
                <li class="icon" v-for="element in social_icons" :key="element">
                    <a href="element.url">
                        <img :src="getImageByURL(element.src)" alt="element.name" class="social_icon">
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<style scoped>


</style>