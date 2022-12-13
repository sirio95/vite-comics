<script>
export default{
    props:{
        img: String,
        descr: String,
        alt: String,
        price: Number
    }
}
</script>

<template>
    <section>
        <div>
            <img :src='img' :alt="alt">
            <p>{{descr}}</p>
            <div>{{price}}</div>
        </div>
    </section>
</template>

<style>

</style>