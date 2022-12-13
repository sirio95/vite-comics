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
            shop: [
                    {text: "shop DC",
                    url: '#',
                    current: false},
                    {text: "shop DC collectibles",
                    url: '#',
                    current: false}
                ],
            terms: [
                    {text: "Terms of Use",
                    url: '#',
                    current: false},
                    {text: "Privacy Policy (New)",
                    url: '#',
                    current: false},
                    {text: "Ad Choices",
                    url: '#',
                    current: false},
                    {text: "Advertising",
                    url: '#',
                    current: false},
                    {text: "Jobs",
                    url: '#',
                    current: false},
                    {text: "Subscriptions",
                    url: '#',
                    current: false},
                    {text: "Talent Workshops",
                    url: '#',
                    current: false},
                    {text: "CPSC Certificates",
                    url: '#',
                    current: false},
                    {text: "Ratings",
                    url: '#',
                    current: false},
                    {text: "Shop Help",
                    url: '#',
                    current: false},
                    {text: "Contact Us",
                    url: '#',
                    current: false}    
            ],
            sites: [
                    {text: "DC",
                    url: '#',
                    current: false},
                    {text: "MAD magazines",
                    url: '#',
                    current: false},
                    {text: "DC Kids",
                    url: '#',
                    current: false},
                    {text: "DC Universe",
                    url: '#',
                    current: false},
                    {text: "DC Power Visa",
                    url: '#',
                    current: false}
                ],
        }
    }
}
</script>

<template>
    <div class="lista">
        <h3>DC COMICS</h3>
        <ul class="links">
            <li v-for="(element, index) in pages" :key="index"><a href="element.url">{{element.text}}</a></li>
        </ul>
    </div>
    <div class="lista">
        <h3>SHOP</h3>
        <ul class="links">
            <li v-for="(element, index) in shop" :key="index"><a href="element.url">{{element.text}}</a></li>
        </ul>
    </div>
    <div class="lista">
        <h3>DC</h3>
        <ul class="links">
            <li v-for="(element, index) in terms" :key="index"><a href="element.url">{{element.text}}</a></li>
        </ul>
    </div>
    <div class="lista">
        <h3>SITES</h3>
        <ul class="links">
            <li v-for="(element, index) in sites" :key="index"><a href="element.url">{{element.text}}</a></li>
        </ul>
    </div>
</template>

<style>

</style>