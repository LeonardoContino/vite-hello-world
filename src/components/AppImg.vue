<script>
 export default {
    data(){
        name : 'Appimages'
        return{
            image: 'download.png'
        }
    },
    methods: {
        GetImageUrl(image){
            const url = new URL(`../assets/${image}`, import.meta.url);
            return url.href;
        }
        }
 }
</script>

<template>
 <img :src="GetImageUrl(image)" alt="">
</template>
<style>

</style>