<template lang="">
    <div class="allcont flex bg-[#F9F9F9] flex-col justify-center ">
       <div v-if="openpop == true" class="popup fixed top-0 left-0 bottom-0 right-0 bg-black z-[99] bg-opacity-[75%] flex justify-center items-center">
            <div class="backgroundd bg-white flex-col lg:flex-row lg:overflow-hidden  overflow-y-scroll w-[343px] 2xl:w-[70%] xl:w-[70%] lg:w-[80%]  h-[80%] flex   lg:h-[90%] rounded-[16.22px]">
                <div class="downloads flex-grow   lg:h-full justify-center items-center  flex">
                    <div class="col flex py-8 flex-col">
                        <div @click="openpop = !openpop" class="close flex lg:hidden z-[99] absolute right-[-15px] top-3 cursor-pointer ">
                            <img src="/icons/close.svg" alt="">
                        </div>
                        <h1 class="text-[28px] pt-3 relative lg:bottom-3 font-bold text-[#282529]">Download App Now!</h1>

                        <div class="steps ">
                            <div class="phone flex py-1  items-center">
                                <img class="w-[16px] h-[16px]" src="/icons/phone.svg" alt="">
                                <p class="text-[14px] px-1.5 font-normal text-[#5E5C61]">Open your iPhone</p>
                            </div>
                            <div class="phone py-1 flex  items-center">
                                <img class="w-[16px] h-[16px]" src="/icons/share.svg" alt="">
                                <p class="text-[14px] px-1.5 font-normal text-[#5E5C61]">Access to camera</p>
                            </div>
                            <div class="phone flex py-1  items-center">
                                <img class="w-[16px] h-[16px]" src="/icons/qrcode.svg" alt="">
                                <p class="text-[14px] px-1.5 font-normal text-[#5E5C61]">Scan QR Code</p>
                            </div>
                            <div class="phone flex py-1  items-center">
                                <img class="w-[16px] h-[16px]" src="/icons/stars.svg" alt="">
                                <p class="text-[14px] px-1.5 font-normal text-[#5E5C61]">Download app and enjoy!</p>
                            </div>

                            <div class="qrcode mt-4 flex py-2 justify-center items-center">
                                <img src="/icons/Qrcode.png" alt="">
                            </div>
                            <div class="qrcode mt-4 flex py-2 justify-center items-center">
                                <div class="list ls flex w-[229px] h-[48px] text-center justify-center text-white rounded-[69px] bg-[#5A45D6] text-[14px]">
                                    <button class=" font-medium text-[16px]">Watch Faces App</button>
                                </div>

                            </div>
                        </div>

                    </div>

                </div>
                <div class="dsg  lg:w-[55%]  h-full">
                    <div @click="openpop = !openpop" class="close hidden lg:flex z-[99] absolute right-8 top-5 cursor-pointer ">
                        <img src="/icons/close.svg" alt="">
                    </div>
                    <img class="w-full h-full hidden lg:flex realtive rounded-[16.22px] " src="/Framepopup.png" alt="">
                    <img class="w-full h-full realtive rounded-[16.22px] " src="/Framepop.png" alt="">
                </div>
                
            </div>

       </div>

        <div class="content w-full flex-wrap justify-center sm:flex-nowrap flex lg:justify-between lg:h-[820px] px-[30px] items-center py-[80px] container mx-auto ">
            <div class="leftside w-full lg:pl-20 flex flex-col items-center lg:items-start lg:w-[43%]">
                <p class="par text-[12px] lg:text-[16px] text-[#5E5C61] uppercase  font-normal">Style your watch in second</p>
                <p class="par text-[36px] lg:text-[72px] flex flex-col break-words items-start	 text-[#282529] whitespace-nowrap font-bold">Pick & Match,<span class="sub whitespace-nowrap text-[36px] lg:text-[72px] relative break-normal bottom-6 font-semibold		 italic  text-[#5b45d6ce]">Make your style</span></p>
                <p class="par text-[#5E5C61] text-center lg:text-start text-[14px] lg:text-[18px] w-[344px] lg:w-[507px]">For WatchOS 7: Discover and Share coolest Watch Faces on the planet for your Apple Watch created by a community of Apple Watch lovers.</p>
                <div @click="openpop = !openpop" class="btns cursor-pointer my-8">
                    <button class="par   flex justify-center text-white bg-[#5A45D6]  w-[200px] h-[50px] rounded-[100px] items-center text-[16px]">Download Now</button>
                </div>
            </div>
            <div class="rightside w-full mt-[100px] lg:mt-0 lg:w-[60%] flex  justify-center">

                <p class="lg:flex hidden w-[430px] min-w-[350px] min-h-[350px] h-[430px] bg-[#FFC947] rounded-full">
                    <svg width="540" height="500" viewBox="0 0 550 550" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <mask id="mask0_7_1189" style="mask-type:alpha" maskUnits="userSpaceOnUse" x="0" y="0" width="550" height="550">
                        <circle cx="274.944" cy="275.176" r="274.5" fill="#FFC947"/>
                        </mask>
                        <g mask="url(#mask0_7_1189)">
                        <g opacity="0.2">
                        <circle cx="233.21" cy="267.862" r="324.84" stroke="white" stroke-width="3.44201"/>
                        <path d="M506.899 267.862C506.899 419.014 384.227 541.55 232.899 541.55C81.5713 541.55 -41.1007 419.014 -41.1007 267.862C-41.1007 116.71 81.5713 -5.82563 232.899 -5.82563C384.227 -5.82563 506.899 116.71 506.899 267.862Z" stroke="white" stroke-width="3.44201"/>
                        <path d="M462.607 267.862C462.607 394.902 359.76 497.884 232.897 497.884C106.034 497.884 3.18707 394.902 3.18707 267.862C3.18707 140.823 106.034 37.8406 232.897 37.8406C359.76 37.8406 462.607 140.823 462.607 267.862Z" stroke="white" stroke-width="3.44201"/>
                        <circle cx="233.21" cy="268.486" r="195.089" stroke="white" stroke-width="3.44201"/>
                        </g>
                        </g>
                        </svg>
                </p>
                <p class="flex lg:hidden  min-w-[350px] min-h-[350px] bg-[#FFC947] rounded-full">
                    <svg width="350" height="350" viewBox="0 0 550 550" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <mask id="mask0_7_1189" style="mask-type:alpha" maskUnits="userSpaceOnUse" x="0" y="0" width="550" height="550">
                        <circle cx="274.944" cy="275.176" r="274.5" fill="#FFC947"/>
                        </mask>
                        <g mask="url(#mask0_7_1189)">
                        <g opacity="0.2">
                        <circle cx="233.21" cy="267.862" r="324.84" stroke="white" stroke-width="3.44201"/>
                        <path d="M506.899 267.862C506.899 419.014 384.227 541.55 232.899 541.55C81.5713 541.55 -41.1007 419.014 -41.1007 267.862C-41.1007 116.71 81.5713 -5.82563 232.899 -5.82563C384.227 -5.82563 506.899 116.71 506.899 267.862Z" stroke="white" stroke-width="3.44201"/>
                        <path d="M462.607 267.862C462.607 394.902 359.76 497.884 232.897 497.884C106.034 497.884 3.18707 394.902 3.18707 267.862C3.18707 140.823 106.034 37.8406 232.897 37.8406C359.76 37.8406 462.607 140.823 462.607 267.862Z" stroke="white" stroke-width="3.44201"/>
                        <circle cx="233.21" cy="268.486" r="195.089" stroke="white" stroke-width="3.44201"/>
                        </g>
                        </g>
                        </svg>
                </p>
                <div class="phone absolute flex items-end">
                    <img class=" absolute" src="/Screen.png" alt="">
                    <img class="rounded-3xl w-[220px] h-[460px] relative bottom-7 " src="/image5.png" alt="">

                    <div class="swatch relative right-10 bottom-7 ">
                        <img src="/Apple.png " class="lg:w-[170px] w-[200px] lg:h-[250px]" alt="">
                    </div>
                    
                </div>
                
                
            </div>
            
        </div>
    </div>
    <div class="divier lg:flex hidden absolute bottom-1 left-0 right-0">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 220"><path fill="#fff" fill-opacity="1" d="M0,128L80,138.7C160,149,320,171,480,176C640,181,800,171,960,176C1120,181,1280,203,1360,213.3L1440,224L1440,320L1360,320C1280,320,1120,320,960,320C800,320,640,320,480,320C320,320,160,320,80,320L0,320Z"></path></svg>
    </div>
    
</template>
<script>
export default {
    data() {
        return {
            openpop:false,
        }
    },
}
</script>
<style scoped>
@import url('https://fonts.cdnfonts.com/css/sf-pro-display');
.par {
    font-family: 'SF Pro Display', sans-serif;
    font-style: normal;
}
.sub{
    
}
    
</style>
