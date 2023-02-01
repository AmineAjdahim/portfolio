<template lang="">
    <div v-if="openmenu == true" class="menu fixed w-full lg:hidden top-[80px] bottom-0 right-0 bg-white z-[99]  flex justify-center items-center">
        <div class="list w-full h-full flex items-center justify-between flex-col py-14">
            <div class="menu flex flex-col items-center">
                <h1 class="text-[30px] font-bold py-4 ls text-[#5A45D6]">Home</h1>
                <h1 class="text-[30px] font-normal py-4 ls text-[#706E72]">Blog</h1>
                <h1 class="text-[30px] font-normal py-4 ls text-[#706E72]">Contact</h1>

            </div>
            <div class="download bg-[#5A45D6] flex justify-center items-center w-[310px] h-[56px] rounded-[100px]">
                <h1 class="text-[18px] font-semibold text-white ls">Download Now</h1>
            </div>
        </div>
        <!-- <h1>ksjdhfisdjhfi</h1> -->
    </div>
    <div class="nav w-full bg-[#F9F9F9] flex items-center min-h-[80px] max-h-[80px] ">
        
        <div class="allnavs justify-between container flex items-center mx-auto px-4 py-1">
            <div class="logo-title flex  items-center">
                <div class="logo w-[30px]">
                    <img class="w-[30px]" src="/logo.svg" alt="">
                </div>
                <div class="tit text-[22px] px-2">
                    <h1>Watch Faces</h1>
                </div>
        
            </div>
            <div class="list  text-[16px] flex-col hidden lg:flex">
                <div class="lo flex justify-center ">
                    <li class="ls flex justify-center flex-col item-center cursor-pointer px-[28px]" v-for="list in listofnav" :key="list.id">
                       <p> {{list.title}} </p>
                       
                       <p v-if="list.title == 'Home'" class="flex  w-[28px] justify-center  mx-auto h-[1px]  bg-[#5A45D6]"></p>
                    </li>
                </div>
            </div>
            <div class="list ls hidden lg:flex w-[160px] h-[40px] text-center justify-center text-white rounded-[69px] bg-[#5A45D6] text-[14px]">
                <button>Try it Now</button>
            </div>
            <div class="vector lg:hidden flex">
                <div v-if="openmenu == false" @click="openmenu = !openmenu" class="vec1">
                    <svg width="26" height="18" viewBox="0 0 26 18" fill="none" xmlns="http://www.w3.org/2000/svg">
                         <path d="M1 9H25M1 1H25M9 17H25" stroke="black" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                    </svg>
                </div>
                <div v-if="openmenu == true" @click="openmenu = !openmenu" class="vec2 ">
                    <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M8 8L24 24M24 8L8 24L24 8Z" stroke="black" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                    </svg>
                </div>

            </div>
            
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            listofnav:[{title:"Home"},{title:"Blog"},{title:"Contact"}],
            openmenu:false,
        }
    },
    
}
</script>
<style scoped>
@import url('https://fonts.cdnfonts.com/css/hk-groteks');
@import url('https://fonts.cdnfonts.com/css/sf-pro-display');

.tit {
    font-family: 'HK Grotesk', sans-serif;
    font-weight: 700;

}
.ls{
    font-family: 'SF Pro Display', sans-serif;
                                                
}
</style>
