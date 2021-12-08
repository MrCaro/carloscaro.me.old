<template>
    <section id="about" class="">
        <div class="container grid grid-col-1 md:grid-cols-2 h-full px-16 gap-y-48">
            <div class="relative flex flex-col items-center justify-center">
                <div class="relative">
                    <img 
                        :src="`${publicPath}icons/squaredot-pattern.svg`" 
                        :srcset="`${publicPath}icons/squaredot-pattern.svg`" 
                        alt=""
                        class="absolute top-[-2rem] left-[-4rem]"
                    >
                    <img 
                        :src="`${publicPath}icons/squaredot-pattern.svg`" 
                        :srcset="`${publicPath}icons/squaredot-pattern.svg`" 
                        alt=""
                        class="absolute bottom-[-1rem] right-[-3rem] "
                    >
                    <img 
                        :src="`${publicPath}img/charlie-headshot-about@2x.png`" 
                        :srcset="`${publicPath}img/charlie-headshot-about@2x.png`" 
                        alt="Charlie headshot"
                        class="headshot relative h-[372px] w-auto"
                        style="filter: drop-shadow(11px 11px 10px #00000029);"
                    >
                    <div class="absolute left-[-3rem] bottom-[5rem] flex justify-center items-center">
                        <div class="absolute h-full w-full filter blur-[0.5px] rounded-xl" style="background: linear-gradient(135deg, #ffffff, #ababab40);"></div>
                        <div class="relative h-auto w-auto px-20 py-12">
                            <p class="text-28">
                                🇻🇪
                            </p> 
                        </div>
                    </div>
                </div>
            </div>
            <div class="flex flex-col justify-center gap-y-20">
                <h2 class="font-univia text-40 text-gray-dark leading-tight">
                    About
                    <span 
                        class="text-white"
                        style="text-shadow: -1px -1px 0 #b928e5, 1px -1px 0 #b928e5, -1px 1px 0 #b928e5, 1px 1px 0 #b928e5;"
                        
                    >
                        Me.
                    </span>
                </h2>
                <p class="font-roboto font-400 text-gray-default mt-32">
                    My name is Carlos but my friends call me Charlie. I'm a Web Dev from Caracas, Venezuela currently living in the Sunshine State and where dreams do come true, you guessed it, that would be Orlando, FL. While in SouthFlo I'm pursuing my MS in Computer Science
                    at UCF. I work as a Web Developer for a Digital shop at Philly called, <a href="https://tasty.studio/" target="_blank" class="underline transition duration-500 ease-in-out hover:text-grape">Tasty Studio LLC 👅 </a>
                </p>
                <p class="font-roboto font-400 text-gray-default">
                    As a passionate developer I'm always in the look to improve my skills and learn new skills. Which leaded me to dig into
                    VR dev. At the moment I've had experience with Unity + SteamVR (I'll add some cool projects on this site soon 🤞). My main goal is to create custom VR applications and add 3D components
                    to web projects at Tasty Studio.
                </p>
                <p class="font-roboto font-400 text-gray-default">
                    While not coding or geeking out about tech you can find me working out or hanging out with friends. 
                </p>
            </div>    
        </div>
    </section>
</template>
<script>
export default {
    name: "About",
    data () {
        return {
            publicPath: process.env.BASE_URL
        }
    },
}
</script>