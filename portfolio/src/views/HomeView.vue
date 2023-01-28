<template lang="">
  <div class="countainer w-full h-screen bg-[#dfe2fd]">
    <div class="menu">
      <Menus/>
  </div>
  <div class="about">
    <About />
  </div>
  <div class="skills mt-32 ">
     <Skills />
  </div>
  </div>
  
</template>
<script>
import Menus from '../components/Menu.vue';
import About from '../components/About.vue';
import Skills from '../components/Skills.vue'
export default {
  components:{
    Menus,
    About,
    Skills,
  },  
  
}
</script>
<style lang="">
  
</style>