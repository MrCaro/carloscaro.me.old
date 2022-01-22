<template>
    <section id="skills" class="">
        <div class="relative container grid grid-col-1 md:grid-cols-2 h-full px-16 gap-y-48">
            <div class="flex flex-col gap-y-20">
                <h2 class="font-univia text-40 text-gray-dark leading-tight">
                    Tech stack that I've used for professional or academic projects.
                </h2>
                <p class="font-roboto font-400 text-gray-default">
                    *for specifics you can refer to highlighted projects and check the tech stack used.
                </p>
            </div>
            <div>
                <img 
                    :src="`${publicPath}img/skills-banner.svg`" 
                    :srcset="`${publicPath}img/skills-banner.svg`" 
                    alt=""
                    class="relative md:absolute transform scale-125"
                >
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: "Skills",
    data () {
        return {
            publicPath: process.env.BASE_URL
        }
    }
}
</script>