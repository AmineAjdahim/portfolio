<template lang="">
    <div class="footer w-full bg-white flex flex-col lg:flex-row items-center lg:justify-between rounded-t-3xl border-t-[1px] border-[#CBCBCB] ">
        <div class="social  flex flex-col h-full justify-between ">
            <div class="logoandsocial flex flex-col px-20 py-14 ">
                <div class="logotitle relative bottom-3  flex">
                    <div class="logo  w-[30px]">
                        <img class="w-[38.76px] lg:w-[33.76px]" src="/logo.svg" alt="">
                    </div>
                    <div class="tit text-[22px] fl px-2">
                        <h1 class="text-[26.62px] lg:text-[24.12px] text-black font-bold tit">Watch Faces</h1>
                    </div>
                </div>
                <div class="list ls  flex-grow flex lg:hidden  ">
                    <button class="w-[180px] h-[40px] text-center text-white rounded-[69px] bg-[#5A45D6] text-[14px]">Try it Now</button>
                </div>
                <div class="social mt-4 flex lg:justify-start justify-center">
                    <img class=" pr-3.5" src="/social/telegram.svg" alt="">
                    <img class=" pr-3.5" src="/social/twitter.svg" alt="">
                    <img class=" pr-3.5" src="/social/facebook.svg" alt="">
                </div>

            </div>
            <!-- <div class="copy  px-20 ">
                <p class="text-[14px] text-[#5E5C61]">2023. Watch Faces. All rights reserved.</p>
            </div> -->

        </div>
        <div class="content  flex-col lg:flex hidden relative lg:top-3 bottom-7 lg:flex-row  w-[60%] py-14 px-20">
            <div class="home  px-5 flex-grow  items-start flex-col">
                <h1 class="text-[18px] par font-semibold text-[#282529]">Home</h1>
                <div class="list mt-2">
                    <p class="par font-normal text-[16px] text-[#5E5C61]">Download App</p>
                    <p class="par font-normal text-[16px] text-[#5E5C61]">Blog</p>
                </div>
            </div>
            <div class="home flex-grow flex items-start flex-col">
                <h1 class="text-[18px] par font-semibold text-[#282529]">Company</h1>
                <div class="list mt-2">
                    <p class="par font-normal text-[16px] text-[#5E5C61]">FAQ</p>
                    <p class="par font-normal text-[16px] text-[#5E5C61]">Contact</p>
                    <p class="par font-normal text-[16px] text-[#5E5C61]">Term of Services</p>
                    <p class="par font-normal text-[16px] text-[#5E5C61]">Privacy Policy</p>
                </div>
            </div>
            
            <div class="list ls lg:flex flex-grow hidden  ">
                <button class="w-[180px] h-[40px] text-center text-white rounded-[69px] bg-[#5A45D6] text-[14px]">Try it Now</button>
            </div>
        </div>

        <!-- mobile -->

        <div class="lis lg:hidden w-full">
            <div class="allfooter">
                <div class="title flex justify-center ">
                    <h1 @click="clickhome = !clickhome" class="text-[18px] par font-semibold text-[#282529] px-1  border-b-[1px] w-[90%] border-[#CBCBCB] flex justify-between"><span class="py-3 text-[18px] text-black font-medium">Home</span> <img src="/row.svg" alt=""> </h1>
                </div>
                <div v-if="clickhome" class="list mt-2 px-7">
                    <p class="par py-1 font-normal text-[16px] text-[#5E5C61]">Download App</p>
                    <p class="par py-1 font-normal text-[16px] text-[#5E5C61]">Blog</p>
                </div>
            </div>
            <div class="allfooter">
                <div class="title flex justify-center ">
                    <h1 @click="clickCompany = !clickCompany" class="text-[18px] par font-semibold text-[#282529] px-1 border-b-[1px] w-[90%] border-[#CBCBCB] flex justify-between"><span class="mt-3 py-3 text-[18px] text-black font-medium">Company</span> <img src="/row.svg" alt=""> </h1>
                </div>
                <div v-if="clickCompany" class="list mt-2 px-7">
                    <p class="par py-1 font-normal text-[16px] text-[#5E5C61]">FAQ</p>
                    <p class="par py-1 font-normal text-[16px] text-[#5E5C61]">Contact</p>
                    <p class="par py-1 font-normal text-[16px] text-[#5E5C61]">Term of Services</p>
                    <p class="par py-1 font-normal text-[16px] text-[#5E5C61]">Privacy Policy</p>
                </div>
            </div>

        </div>

    </div>
</template>
<script>
export default {
    data() {
        return {
            clickhome:false,
            clickCompany:false,
        }
    },
    mounted() {
        // console.log("click  :" this.clickhome);
    }

}
</script>
<style scoped>
@import url('https://fonts.cdnfonts.com/css/hk-groteks');
@import url('https://fonts.cdnfonts.com/css/sf-pro-display');

.tit {
    font-family: 'HK Grotesk', sans-serif;
}
.par{
    font-family: 'SF Pro Display', sans-serif;
                                                
}
</style>