<script>

import AppSubstring from './components/AppSubstring.vue';
import AppBanner from './components/AppBanner.vue';

export default{
  data() {
    return{
      announcement : "La mia prima app con Vite!"
    }
  },

  components:{
     AppSubstring,
     AppBanner

  },

  methods:{

  }

}
</script>

<template>
<h1>{{ announcement }}</h1>
<AppSubstring></AppSubstring>
<AppBanner></AppBanner>
</template>

<style scoped>


h1{
  color: chocolate;
  background-color: black;
  padding: 2rem;
  text-align: center;
  font-size: 4rem;
  margin: 0 auto;
}

</style>
