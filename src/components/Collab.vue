<template>
    <section class="">
        <div class="container grid grid-col-1 h-full px-16 gap-y-20 text-center">
            <h2 class="font-univia text-40 text-gray-dark leading-tight">
                👨‍💻 Collab?
            </h2>
            <p class="font-roboto font-400 text-gray-default">
                If you have any questions about how Tasty Studio or myself can help you or you just want to connect. <br>
                Don't hesitate to go ahead and reach out! Looking forward to talk. 
            </p>
            <div class="w-[fit-content] m-auto mt-52">
                <MainCTA 
                    url="mailto:carocarlosj@gmail.com" 
                    title="Let's talk"
                />
            </div>
        </div>
    </section>
</template>
<script>
    import MainCTA from "@/components/MainCTA.vue";
    export default {
        name: "Collab",
        components: {
            MainCTA
        },
    }
</script>