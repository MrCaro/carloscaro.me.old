<template>
    <section class="bg-gray-light pt-52 pb-60">
        <div class="container grid grid-col-1 md:grid-cols-2 h-full px-16 gap-y-48">
            <div class="flex flex-col justify-center gap-y-20">
                <h1 class="font-univia text-60 text-gray-dark leading-tight">
                    Web & VR <br>
                    <span 
                        class="text-gray-light"
                        style="text-shadow: -1px -1px 0 #b928e5, 1px -1px 0 #b928e5, -1px 1px 0 #b928e5, 1px 1px 0 #b928e5;"
                        
                    >
                        Developer.
                    </span>
                </h1>
                <p class="font-roboto font-400 text-gray-default">
                    Inexpensive development can be expensive in the long term.
                </p>
            </div>
            <div class="relative flex flex-col items-center justify-center">
                <div class="relative">
                    <img 
                        :src="`${publicPath}icons/squaredot-pattern.svg`" 
                        :srcset="`${publicPath}icons/squaredot-pattern.svg`" 
                        alt=""
                        class="absolute top-[-2rem] right-[-4rem]"
                    >
                    <img 
                        :src="`${publicPath}icons/squaredot-pattern.svg`" 
                        :srcset="`${publicPath}icons/squaredot-pattern.svg`" 
                        alt=""
                        class="absolute bottom-[-1rem] left-[-3rem] "
                    >
                    <img 
                        :src="`${publicPath}img/charlie-headshot-hero@2x.png`" 
                        :srcset="`${publicPath}img/charlie-headshot-hero@2x.png`" 
                        alt="Charlie headshot"
                        class="relative h-[372px] w-auto"
                        style="filter: drop-shadow(11px 11px 10px #00000029);"
                    >
                    <div id="GlassBox1" class="absolute left-[-75%] top-[9rem] flex justify-center items-center">
                        <div class="absolute h-full w-full filter blur-[0.5px] rounded-xl" style="background: linear-gradient(135deg, #ffffff, #ababab40);"></div>
                        <div class="relative h-auto w-auto p-16 flex items-center gap-16">
                            <div>
                                <p class="text-28">
                                    💡
                                </p>
                            </div>
                            <div>
                                <p class="font-univia text-14 text-gray-dark leading-tight">
                                    Looking for?
                                </p> 
                                <p 
                                    class="font-roboto font-400 text-gray-default text-12 mt-6"
                                    style="width: 21ch"
                                >
                                    Custom website / E-commerce or UI design.
                                </p>
                            </div>
                        </div>
                    </div>
                    <div class="absolute right-[2rem] bottom-[-1rem] flex justify-center items-center">
                        <div class="absolute h-full w-full filter blur-[0.5px] rounded-xl" style="background: linear-gradient(135deg, #ffffff, #ababab40);"></div>
                        <div class="relative h-auto w-auto px-20 py-12">
                            <p class="text-28">
                                👋
                            </p> 
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: "MainHero",
    data () {
        return {
            publicPath: process.env.BASE_URL
        }
    },
}
</script>