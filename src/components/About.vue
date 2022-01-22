<template>
    <section id="about" class="">
        <div class="container grid grid-col-1 md:grid-cols-2 h-full px-16 gap-y-48">
            <div class="relative flex flex-col items-center justify-center order-2 md:order-1">
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
            <div class="flex flex-col justify-center gap-y-20 order-1 md:order-2">
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
                    Hi I'm Charlie and I'm a Web Developer at <a href="https://tasty.studio/" target="_blank" class="underline transition duration-500 ease-in-out hover:text-grape">Tasty Studio 👅</a>. Currently I'm pursuing my Master's Degree in Computer Science with a specialization in MX Reality at UCF, Orlando FL.
                </p>
                <p class="font-roboto font-400 text-gray-default">
                    My main goal as a developer is to combine my Front End Engineer and 3D skills to craft digital ideas that can not only elevate user experience but 
                    ultimately creating robust and user friendly tools. As an individual I would describe myself as a sapien that is constantly upgrading themself to 
                    be the best possible version of him. But hey, life is too short, therefore I don't (try to at least haha) not taking it too serious and enjoy each day
                    as it is, a gift!
                </p>
                <p class="font-roboto font-400 text-gray-default">
                    <span class="text-gray-default">Hometown /</span> Caracas, Venezuela
                    <br>
                    <span class="text-gray-default">Colors / </span><span class="inline-block h-16 w-16 rounded-full bg-grape"></span> <span class="inline-block h-16 w-16 rounded-full -ml-8 bg-[#F202F2]"></span>
                    <br>
                    <span class="text-gray-default">Teams /</span> Chelsea FC ⚽️  NETS 🏀  Marlins & Red Sox ⚾️
                    <br>
                    <span class="text-gray-default">Hobbies /</span> 🎮 🏋️‍♀️ 🏃‍♂️ ⚽️ 📚
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
    }
}
</script>