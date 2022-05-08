<template>
  <section id="skills" class="">
    <div class="relative container grid grid-col-1 h-full px-16 gap-y-48">
      <div class="flex flex-col">
        <h2 class="font-univia text-40 text-gray-dark leading-tight">
          Technical
          <span
            class="text-white"
            style="text-shadow: -1px -1px 0 #b928e5, 1px -1px 0 #b928e5, -1px 1px 0 #b928e5, 1px 1px 0 #b928e5;"
            >Skills</span
          >
          Within Charlie's Utility Belt
        </h2>
        <p class="font-roboto font-400 text-gray-default text-14 mt-20">
          For specifics you can refer to highlighted projects and check the tech
          stack.
        </p>
      </div>
      <div class="grid grid-cols-3">
        <div class="">
          <p class="font-univia text-12 text-gray-dark leading-tight mt-20">
            Web Development / Design
          </p>
          <ul class="font-roboto font-400 text-gray-default text-12">
            <li>TailwindCSS</li>
            <li>Twig</li>
            <li>VueJS</li>
            <li>Shopify</li>
            <li>WordPress</li>
            <li>Adobe XD</li>
            <li>Figma</li>
          </ul>
        </div>
        <div>
          <p class="font-univia text-12 text-gray-dark leading-tight mt-20">
            VR
          </p>
          <ul class="font-roboto font-400 text-gray-default text-12">
            <li>Unity</li>
            <li>SteamVR</li>
          </ul>
        </div>
        <div>
          <p class="font-univia text-12 text-gray-dark leading-tight mt-20">
            AR
          </p>
          <ul class="font-roboto font-400 text-gray-default text-12">
            <li>Unity</li>
            <li>Vuforia</li>
          </ul>
        </div>
      </div>
      <div class="relative h-[148px] lg:h-[332px]">
        <img
          :src="`${publicPath}img/skills-banner-2.svg`"
          :srcset="`${publicPath}img/skills-banner-2.svg`"
          alt=""
          class="relative md:absolute transform scale-125"
        />
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: "Skills",
  data() {
    return {
      publicPath: process.env.BASE_URL,
    };
  },
};
</script>
