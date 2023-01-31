<template lang="">
    <div class="layout w-full flex justify-center flex-col py-8 bg-[#F5F5F5]">
        <div class="title">
            <h1 class="flex flex-col items-center"> <span class="par text-[64px] font-bold text-[#282529]"> Don’t take our word for it.</span>
               <span class="par  text-[#5A45D6] text-[64px] font-semibold italic">Trust our customers!</span></h1>
        </div>
        <div class="allcarts w-full px-20 flex flex-wrap py-8 ">
            <div class="cart flex flex-wrap">
                <div v-for="client in clients" class="carrs w-[378px]  my-2 mx-1  ">
                    <div class="bo bg-white rounded-[15px] flex">
                        <div class="img px-5 py-5">
                            <img :src="client.img" alt="asas">
                        </div>
                        <div class="content py-5">
                            <p class="text-[#462C5B] font-semibold text-[16px] par ">{{client.fullname}}</p>
                            <p class="work text-[14px] text-[#58585E]">{{client.work}}</p>
                            <div class="allstar flex">
                                <div v-for="star in 5" class="star flex ">
                                    <img v-if="client.star >= star" class="w-[11.57px] h-[11.2px]" src="/Star_light.png" alt="">
                                    <img v-if="client.star < star" class="w-[11.57px] h-[11.2px]" src="/Star.png" alt="">
                                </div>
        
                            </div>
                            <div class="description w-[266px]">
                                <p class="text-[14px] text-[#282529] font-normal pt-3 pr-5">{{client.description}}</p>
                            </div>
                        </div>

                    </div>

                </div>
    
            </div>

        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            clients:[
                {fullname:"Nahid Hasan",img:"/characters/charcters1.png",work:"UX/UI Designer",star:3,description:"UI is the saddle, the stirrups, & the reins. UX is the feeling you get being able to ride the horse."},
                {fullname:"Nahid Hasan",img:"/characters/charcters2.png",work:"UX/UI Designer",star:4,description:"UI is the saddle, the stirrups, & the reins. UX is the feeling you get being able to ride the horse. UI is the saddle, the stirrups, & the reins. UX is the feeling you get being able to ride the horse. UI is the saddle, the stirrups, & the reins. "},
                {fullname:"Nahid Hasan",img:"/characters/charcters3.png",work:"UX/UI Designer",star:3,description:"UI is the saddle, the stirrups, & the reins. UX is the feeling you get being able to ride the horse."},
                {fullname:"Nahid Hasan",img:"/characters/charcters4.png",work:"UX/UI Designer",star:1,description:"UI is the saddle, the stirrups, & the reins. UX is the feeling you get being able to ride the horse."},
                {fullname:"Nahid Hasan",img:"/characters/charcters5.png",work:"UX/UI Designer",star:2,description:"UI is the saddle, the stirrups, & the reins. UX is the feeling you get being able to ride the horse."},
                {fullname:"Nahid Hasan",img:"/characters/charcters6.png",work:"UX/UI Designer",star:3,description:"UI is the saddle, the stirrups, & the reins. UX is the feeling you get being able to ride the horse."},
            
            ],
        }
    },
    
}
</script>
<style scoped>
@import url('https://fonts.cdnfonts.com/css/sf-pro-display');

.par {
    font-family: 'SF Pro Display', sans-serif;
    /* font-style: normal; */
}

    
</style>