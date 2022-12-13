<script>
export default{
    props:{
        img: String,
        descr: String,
        alt: String,
        price: Number,
    }
}
</script>

<template>

    <div class="card">
        <img :src='img' :alt="alt">
        <p>{{descr}}</p>
        <div class="price_tag">{{price}}</div>
    </div>
</template>

<style lang="scss" scoped>
    @use "../../assets/scss/variables.scss";

    
    .card{
        flex-basis: calc((100% - 100px - 60px) / 6);
        max-height: 200px;
        margin: 40px 5px;
        padding:2px;
        position:relative;

            img{
                width: 80%;
                max-height: 70%;
            }
            p{
                font-size:0.8rem;
                margin:0;
            }
            .price_tag{
                width: 100px;
                height:50px;
                background-color:#fff;
                opacity: 0.8;
                color:red;
                position:absolute;
                top:40%;
                left:20%;
                display:none;
            }
    }
</style>