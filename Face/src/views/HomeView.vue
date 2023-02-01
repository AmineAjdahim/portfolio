<template lang="">
  <div class="homepage w-full h-screen ">
    
    <div class="h1  w-full  h-screen">
      
      <div class="nav container mx-auto px-4">
        <Navbar/>
      </div>
      <div class="cont">
        <div class="content ">
        <Hero />
        </div>
        <div class="Most py-6 text-[64px] bg-[#F5F5F5]">
          <Most_Popular/>
        </div>
        <div class="client py-6 text-[64px] bg-[#F5F5F5]">
          <client_review/>
        </div>
        <div class="ads py-6 text-[64px] bg-[#F5F5F5]">
          <ads/>
        </div>
        <div class="ads py-6 text-[64px] bg-[#F5F5F5]">
          <Footer/>
        </div>
      </div>
    </div>
  </div>
  
</template>
<script>
import Navbar from '../components/Navbar.vue';
import Hero from '../components/Hero.vue';
import Most_Popular from '../components/Most_Popular.vue';
import client_review from '../components/Client_review.vue';
import Ads from '../components/Ads.vue';
import Footer from '../components/Footer.vue'
export default {
  data() {
    return {
      
    }
  },
  components:{
    Navbar,
    Hero,
    Most_Popular,
    client_review,
    Ads,
    Footer
  },  
  
}
</script>
<style scoped>
@import url('https://fonts.cdnfonts.com/css/sf-pro-display');
.divider {
  /* Divider */

}


  
</style>