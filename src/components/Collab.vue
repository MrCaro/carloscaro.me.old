<template>
  <section class="">
    <div class="relative container grid grid-col-1 h-full px-16 gap-y-20 text-center my-32 md:my-64">
      <div 
          data-aos="fade-up"
          data-aos-offset="-300"
          data-aos-anchor-placement="center-center"
        >
        <h2 class="font-univia text-40 text-gray-dark leading-tight">
          👨‍💻 Collab Maybe?
        </h2>
      </div>
      <p class="font-roboto font-400 text-gray-default text-14">
        Don't be shy! I'm sure Charlie is looking forward to chat.
      </p>
      <div class="w-[fit-content] m-auto">
        <MainCTA
          url="mailto:carocarlosj@gmail.com"
          target="_blank"
          title="Let's talk"
        />
      </div>
      <div
        class="absolute top-0 bottom-0 left-0 right-0 m-auto z-[-2] opacity-5 w-[fit-content] h-[fit-content]"
      >
        <svg
          viewBox="0 0 24 24"
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          class="w-[300px] lg:w-[1000px] h-[300px] lg:h-[1000px]"
        >
          <g
            style="animation:loader5 20s linear infinite both;transform-origin:center center"
          >
            <circle cx="12" cy="12" r="4" stroke="#788092" stroke-width="0.5" />
            <circle cx="17" cy="7" r="1" fill="#788092" />
          </g>
        </svg>
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
