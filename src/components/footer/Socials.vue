<script>
export default{
    data(){
        return{
            social_icons: [
                "fa-facebook",
                "fa-twitter",
                "fa-youtube",
                "fa-pinterest-p",
                "fa-location-dot"
            ]            
        }
    },
    addIcons(icon){
        this.innerHTML= icon;
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
                <li class="icon" v-for="element in social_icons" :key="element"><i class="fa-brands" :class="element"></i></li>
            </ul>
        </div>
    </div>
</template>

<style>

</style>