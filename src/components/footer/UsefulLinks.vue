<script>

export default{

    data(){
        return{
            pages: [
                    "characters", "comics", "movies", "tv", "games", "collectibles", "videos", "fans", "news", "shop" 
                ],
            shop: ["shop dc", "shop dc collectibles"],
            terms: ["Terms of Use", "Privacy Policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us"],
            sites: ["DC", "MAD magazines", "DC Kids", "DC Universe", "DC Power Visa"],
        }
    }
}
</script>

<template>
    <div class="lista">
        <h3>DC COMICS</h3>
        <ul class="links" v-for="element in pages" :key="element">
            <li><a href="">{{element}}</a></li>
        </ul>
    </div>
    <div class="lista">
        <h3>SHOP</h3>
        <ul class="links" v-for="element in shop" :key="element">
            <li><a href="">{{element}}</a></li>
        </ul>
    </div>
    <div class="lista">
        <h3>DC</h3>
        <ul class="links" v-for="element in terms" :key="element">
            <li><a href="">{{element}}</a></li>
        </ul>
    </div>
    <div class="lista">
        <h3>SITES</h3>
        <ul class="links" v-for="element in sites" :key="element">
            <li><a href="">{{element}}</a></li>
        </ul>
    </div>
</template>

<style>

</style>