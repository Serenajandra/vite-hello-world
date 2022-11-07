<script>
export default {
        data() {
            return{
                imgName: `halloween.jpg`
            }
        },
        methods:{
            getImgPath(){
                return new URL (`../assets/img/${this.imgName}`, import.meta.url).href;
            }
        }
    }
</script>
<template>
    <div class="banner">
    <img :src="getImgPath()" alt="">
    </div>
</template>
<style scoped>
.banner{
    width: 100%;
    height: 50vh;
    margin: 0 auto;
  }
  
.banner img{
    object-fit: cover;
    width: 100%;
    height: 100%; 
  }
</style>