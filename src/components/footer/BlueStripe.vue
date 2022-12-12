<script>
export default{
    data(){
        return{
            iconsName: [
                {
                    name: "digital domics",
                    src: "buy-comics-digital-comics.png"
                },
                {
                    name: "dc merchandise",
                    src: "buy-comics-merchandise.png"
                },
                {
                    name: "subscription",
                    src: "buy-comics-subscriptions.png"
                },
                {
                    name: "comic shop locator",
                    src: "buy-comics-shop-locator.png"
                },
                {
                    name: "dc power visa",
                    src: "buy-dc-power-visa.svg"
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
    <div id="blue_stripe">
        <ul v-for="element in iconsName" :key="element" id="icons">
            <li>
                <a href="">
                    <img :src="getImageByURL(element.src)" alt="element.name" class="icona">
                    <div class="testo">{{element.name}}</div>
                </a>
            </li>
        </ul>
    </div>


</template>

<style>

</style>