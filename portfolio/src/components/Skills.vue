<template lang="">
    <div class="skillsborder flex justify-center w-full h-full rounded-t-3xl rounded-b-3xl  ">
        <div class="skills w-full h-full flex flex-col items-center mb-12 ">
            <div class="titile mt-7 mb-4 ">
                <h1 class="skillstxt text-[32px] font-bold text-[#2b1e44] ">MySkills</h1>
                <p class="flex w-[120px] h-[4px] rounded-3xl bg-[#9969ef]"></p>
            </div>
            <div class="cart w-[90%] h-full mt-4 flex justify-center flex-wrap">
                    <div v-for="skill in skills" class="carts cursor-pointer borders mx-3 my-3 rounded-3xl p-6 w-[160px] h-[160px] bg-[#1d2741dc] flex justify-center flex-col items-center">
                        <img class="w-[100px] h-[100px]" :src="skill.img" alt="">
                        <h1 class=" text-white font-semibold text text-[20px]">{{skill.name}}</h1>
                    </div>
                    
                
            </div>

        </div>

    </div>
</template>
<script>
import gsap from 'gsap'
import {ScrollTrigger} from 'gsap/ScrollTrigger' 
// gsap.registerPlugin(ScrollTrigger);
export default {
    name:'Skills',
    data() {
        return {
            skills:[
                {name:'C',img:'c-program-icon.svg'},
                {name:'C++',img:'c++.png'},
                {name:'Docker',img:'docker.png'},
                {name:'Linux',img:'linux.png'},
                {name:'Python',img:'python.png'},
                {name:'Javascript',img:'javascript.png'},
                {name:'Typescript',img:'typescript.png'},
                {name:'React.Js',img:'react-icon-29.jpg'},
                {name:'Vue.Js',img:'vuejs.png'},
                {name:'Next.Js',img:'Nextjs.png'},
                {name:'HTML5',img:'html5.png'},
                {name:'CSS3',img:'css3.png'},
                {name:'TailwindCss',img:'tailwind-css.svg'},
                {name:'MongoDb',img:'mongodb.png'},
                {name:'Git/Github',img:'github.png'},
                {name:'Selenium',img:'selenium.svg'},
                {name:'Web Scraping',img:'websc.png'},

            ]
        }
    },
    mounted() {
        gsap.registerPlugin(ScrollTrigger);

        // gsap.to('.skillstxt',{
        //     scrollTrigger:{
        //         trigger: '.skillstxt',
        //         start:"top 80%",
        //         markers:true,
        //     },
        //     x:600,
        //     duration:3
        // });
        gsap.fromTo('.carts',{opacity:0},{
            scrollTrigger:{
                trigger: '.carts',
                start:"top 80%",
                end:'top 1%',
                scrub: 1
            },
            autoAlpha:1,
            stagger:0.6,
            duration:3
        })
    },
    
}
</script>
<style scoped>

.textut {
    font-family: 'Montserrat', sans-serif;
font-family: 'Poppins', sans-serif;
}
.carts:hover {
    transform: scale(1.2);
    background: rgb(236,119,190);
background: linear-gradient(127deg, rgba(236,119,190,1) 23%, rgba(148,104,242,1) 100%);     
}
.carts {
    -webkit-box-shadow: 7px 7px 8px 4px rgba(0,0,0,0.35); 
box-shadow: 7px 7px 8px 4px rgba(0,0,0,0.35);
}


    
</style>