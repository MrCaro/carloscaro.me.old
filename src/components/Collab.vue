<template>
  <section class="">
    <div
      class="container grid grid-col-1 h-full px-16 gap-y-20 text-center mt-64"
    >
      <h2 class="font-univia text-40 text-gray-dark leading-tight">
        👨‍💻 Maybe Collab?
      </h2>
      <p class="font-roboto font-400 text-gray-default text-14">
        If you have any questions about how Charlie can assist you or maybe you
        just want to connect. <br />
        Don't be shy! I'm sure Charlie is looking forward to chat.
      </p>
      <div class="w-[fit-content] m-auto">
        <MainCTA url="mailto:carocarlosj@gmail.com" title="Let's talk" />
      </div>
    </div>
  </section>
</template>
<script>
import MainCTA from "@/components/MainCTA.vue";
export default {
  name: "Collab",
  components: {
    MainCTA,
  },
};
</script>
