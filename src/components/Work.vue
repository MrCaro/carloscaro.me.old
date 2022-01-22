<template>
    <section id="work" class="">
        <div class="container grid grid-col-1 h-full px-16">
            <div class="flex flex-col gap-y-20">
                <h2 class="font-univia text-40 text-gray-dark leading-tight capitalize md:text-center">
                    check out some of my latest
                    <span 
                        class="text-white"
                        style="text-shadow: -1px -1px 0 #b928e5, 1px -1px 0 #b928e5, -1px 1px 0 #b928e5, 1px 1px 0 #b928e5;"
                        
                    >
                        Work. 
                    </span>
                </h2>
                <!-- <div class="relative w-full h-[300px]">
                    <img 
                        :src="`https://source.unsplash.com/random`" 
                        :srcset="`https://source.unsplash.com/random`" 
                        alt=""
                        class="absolute top-0 left-0 w-full h-full object-cover object-center"
                    >
                </div> -->
                <h3 class="font-univia text-30 text-gray-dark leading-tight capitalize text-left mt-64">
                    snow shader
                </h3>
                <div class="grid grid-col-1 md:grid-cols-2">
                    <div class="flex flex-col justify-between">
                        <p class="font-roboto font-400 text-16 text-gray-default m-0">
                            Description
                        </p>
                        <div class="flex items-center text-left mt-16">  
                            <p class="font-roboto font-400 text-14 text-gray-default m-0">
                                Developers  
                            </p>
                            <a 
                                href="https://github.com/MrCaro"
                                target="_blank"
                                rel="noopener noreferrer"
                                class="flex"
                            >
                                <vs-avatar size="medium" src="https://avatars2.githubusercontent.com/u/36524539?s=460&v=4"/>
                            </a>
                        </div>
                    </div>
                    <div>
                        <video 
                            class="video-plyr-component w-full h-full" 
                            src="https://res.cloudinary.com/dbyzfcnpg/video/upload/v1642459842/snow_accumulation.mp4"
                            :poster="`${publicPath}img/snow-accumulation-poster.jpg`"
                        >
                        </video>
                    </div>
                </div>
                <!-- <p class="font-roboto font-400 text-gray-default mt-32 text-left">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Saepe eos a excepturi explicabo quidem fuga. Esse quod consequatur non aspernatur maxime et, voluptas nostrum eveniet quo aut dicta ex dolore!
                </p> -->
                <!-- <vs-button color="success" type="flat" icon="visibility">Done</vs-button>
                <vs-button @click="$vs.notify({title:'Default',text:'Lorem ipsum dolor sit amet, consectetur'})" color="primary" type="border">Notification white</vs-button> -->
                <!-- <hr class="my-32"> -->
                <div class="flex md:justify-center items-center gap-x-16 mt-32">
                    <p class="font-roboto font-400 text-gray-default">
                        upcoming project!
                    </p>
                    <vs-button class="w-[fit-content]" @click="$vs.notify({title:'Coming soon 👀',text:'Tools: Unity and SteamVR',color:'#b928e5'})" color="#b928e5" type="border">VR Escape Room</vs-button>
                    <vs-button class="w-[fit-content]" @click="$vs.notify({title:'Coming soon 👀',text:'Tools: Shopify',color:'#b928e5'})" color="#b928e5" type="border">Bardega Cocktails</vs-button>
                </div>
            </div>
        </div>
    </section>  
</template>

<script>
// import Vue from 'vue'
import Plyr from 'plyr'
import 'plyr/dist/plyr.css'

export default {
    name: "Work",
    data() {
        return {
            publicPath: process.env.BASE_URL
        }
    },
    mounted() {
        document.querySelectorAll('.video-plyr-component').forEach((el) => {
            new Plyr(el, {
                autoplay: false,
                muted: true,
                iconPrefix: 'plyr',
                // controls: false
                // iconUrl: '/wp-content/themes/scripps/src/assets/icons/plyr.svg'
            })
        })
    },
}
</script>