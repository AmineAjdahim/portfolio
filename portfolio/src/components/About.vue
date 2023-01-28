<template lang="">
    <div class="allcart mt-9 w-full h-full flex px-14 ">
        
        <div class="cart grow  flex w-[60%] rounded-3xl h-[420px] ml-[70px] mr-28 bg-[#162036]">
            <div class="side1 w-[35%] h-full bg-white rounded-l-2xl">

            </div>
            <div class="side2 w-[60%]">
                <div class="name mt-10 px-4 mx-2">
                    <p class="aboutme textut text-[#cecece]   mx-1  rounded-3xl py-2 ">About Me</p>
                    <p class="flex w-[70px] h-[1px] rounded-3xl bg-white"></p>


                    <br />
                    <h1 class="myname textut text-white font-bold text-[30px]">Md Amine Ajdahim</h1>

                    <p class="aboutmetext textut px-1 mt-5 text-[14px] text-[#c7c6c6]">
                        Mohammed Amine Ajdahim, a 22-year-old front-end developer,
                         has a passion for creating visually appealing and user-friendly
                          web applications. He is hardworking, reliable, willing to go
                           above and beyond to support team and serve customers. He has a
                            background in cross-platform development, equipped with skills
                             to tackle challenges and known for his problem-solving abilities.
                              He is constantly motivated to learn and grow in his field and
                               believes his technical skills and drive make him an asset to
                                any team.
                    </p>
                    <!-- <h1 class="flex w-[110px] h-[7px] rounded-3xl bg-white mt-2"></h1> -->
                    <div class="btns flex mt-6 textut ">
                        <p><img class="icons cursor-pointer w-[35px]" src="https://img.icons8.com/fluency/48/null/linkedin-circled.png"/></p>
                        <p><img class="icons cursor-pointer w-[35px]" src="https://img.icons8.com/fluency/48/null/instagram-new.png"/></p>
                        <p><img class="icons cursor-pointer w-[35px]" src="https://img.icons8.com/color/48/null/facebook-new.png"/></p>
                        <p><img class="icons cursor-pointer w-[35px]" src="https://img.icons8.com/color/48/null/snapchat-circled-logo--v1.png"/></p>
                        <p><img class="icons cursor-pointer w-[35px]" src="https://img.icons8.com/color/48/null/twitter-circled--v1.png"/></p>
                        
                        <!-- <p class="instagram grow text-white text-center mx-1 font-semibold rounded-3xl py-2 uppercase bg-[#8649f8]"><img src="https://img.icons8.com/clouds/100/null/linkedin.png"/></p>
                        <p class="grow text-white text-center mx-1 font-semibold rounded-3xl py-2 bg-[#1114dc]">facebook</p> -->
                    </div>

                    
                </div>

            </div>
        </div>

    </div>
        <!-- <div class="carts w-[80%] h-[300px]">
asdasd
        </div> -->
        


</template>
<script>
import gsap from 'gsap'
export default {
    name:'about',
    mounted() {
        gsap.fromTo('.cart',{y:50},{y:0,delay:0.7, duration:3})
        gsap.fromTo('.about',{opacity:0},{opacity:1,delay:2})
        // gsap.fromTo('.aboutme',{opacity:0},{opacity:1,delay:3})
        gsap.fromTo('.aboutme',{y:10,opacity:0},{y:0,opacity:1,delay:2,duration:2})
        // gsap.fromTo('.myname',{x:80,opacity:0},{x:0,opacity:1,delay:3,duration:3})
        // gsap.fromTo('.aboutmetext',{y:80,opacity:0},{y:0,opacity:1,delay:3,duration:3})
        gsap.fromTo('.icons',{y:10,opacity:0},{y:0,opacity:1,delay:2,duration:2})

    },
    
}
</script>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital@1&family=Poppins:wght@300&display=swap');
.side1{
    /* background: rgb(148,104,242);
background: linear-gradient(180deg, rgba(148,104,242,1) 23%, rgba(236,119,183,1) 100%); */
background: rgb(236,119,190);
background: linear-gradient(127deg, rgba(236,119,190,1) 23%, rgba(148,104,242,1) 100%);     
}
.cart {
    -webkit-box-shadow: 25px 34px 45px 10px rgba(110,110,110,0.82); 
box-shadow: 25px 34px 45px 10px rgba(110,110,110,0.82);
}
.textut {
    font-family: 'Montserrat', sans-serif;
font-family: 'Poppins', sans-serif;
}
.instagram {
    background: rgb(148,104,242);
background: linear-gradient(90deg, rgba(148,104,242,1) 0%, rgba(252,176,69,1) 50%, rgba(236,119,190,1) 100%);
}

    
</style>