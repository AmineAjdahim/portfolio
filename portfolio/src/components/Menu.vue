<template lang="">
  <div class="menu flex justify-between items-center px-32 py-3">
    <div class="images flex items-center">
        <div class="logo flex w-[50px] h-[50px] rounded-full ">
            <img class=" flex w-[50px] h-[52px] rounded-full " src="profile.png" alt="">
        </div>
        <p class="lis name font-semibold px-4  text-[20px]"> Md Amine Ajdahim</p>

    </div>
    <div class="menu ul flex ">
        <li class="lis font-semibold flex px-4  "   v-for="a in menus"  ><a href="#" v-if="a.color" class="bg-[#0d1639] font-semibold px-5 py-2 rounded-3xl text-white" >{{a.name}} </a><a href="#" v-if="!a.color" class="py-2 font-semibold rounded-2xl hover:bg-[#ffffff] px-5">{{a.name}} </a></li>
    </div>
  </div>
</template>
<script>
import gsap from 'gsap'
export default {
    name:'menu',
    data() {
        return {
            menus:[{name:'About'},{name:'MySkills'},{name:'Myprojects',color:'#0d1639'},{name:'Contacts'}]
        }
    },
    mounted() {
        gsap.fromTo('.proff',{scale:0 },{scale:1,delay:2})
        gsap.fromTo('.logo',{scale:0,y:-60},{scale:1,delay:0.5,y:0,duration:0.7 })
        gsap.fromTo('.lis ',{scale:0,y:-60},{scale:1,delay:0.5,y:0,duration:0.7 })


    },

    
}
</script>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital@1&family=Poppins:wght@300&display=swap');

.lis {
    font-family: 'Montserrat', sans-serif;
font-family: 'Poppins', sans-serif;
}
    
</style>