<template>
  <section id="about" class="relative">
    <div class="container grid grid-col-1 md:grid-cols-2 h-full px-16 gap-y-48">
      <div
        class="relative flex flex-col items-center justify-center order-2 md:order-1"
      >
        <div class="relative">
          <img
            :src="`${publicPath}icons/squaredot-pattern.svg`"
            :srcset="`${publicPath}icons/squaredot-pattern.svg`"
            alt=""
            class="absolute top-[-2rem] left-[-4rem]"
          />
          <img
            :src="`${publicPath}icons/squaredot-pattern.svg`"
            :srcset="`${publicPath}icons/squaredot-pattern.svg`"
            alt=""
            class="absolute bottom-[-1rem] right-[-3rem] "
          />
          <img
            :src="`${publicPath}img/charlie-header-bw.png`"
            :srcset="`${publicPath}img/charlie-header-bw.png`"
            alt="Charlie headshot"
            class="headshot relative h-[372px] w-auto"
            style="filter: drop-shadow(11px 11px 10px #00000029);"
          />
          <div
            class="absolute left-[-3rem] bottom-[5rem] flex justify-center items-center"
          >
            <div
              class="absolute h-full w-full rounded-xl bg-white"
              style="box-shadow: 0 0 5rem 0 rgba(0, 0, 0, .3)"
            ></div>
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
          <span class="title--gradient">
            About
          </span>
          Who? Charlie?
        </h2>
        <p class="font-roboto font-400 text-gray-default mt-32 text-14">
          Carlos/Charlie/Charlos is a Front-End Web Developer at
          <a class="text-gray-dark" href="https://tasty.studio/" target="_blank" rel="noopener noreferrer">Tasty Studio</a
          >. Before moving to Orlando, Charlie spent seven years in Miami, FL
          where he got his Bachelors in Computer Science and Business Management
          from St. Thomas University. Charlie is responsible for bringing digital
          experiences to the www. which can range from e-commerce, marketing
          landing pages, SPA or overall web projects. At Tasty Studio Charlie not
          only craft complex web solutions but also takes part of business
          development in departments like sales & optimization/innovations.
        </p>
        <p class="font-roboto font-400 text-gray-default text-14">
          Currently, Charlie is a full time student at University of Central
          Florida where he is getting a Master's degree in Computer Science
          with a specialization in Mixed Reality Development.
        </p>
        <ul class="font-roboto font-400 text-gray-default text-14">
          <li>
            <span>Colors / </span
            ><span class="inline-block h-14 w-14 rounded-full bg-grape"></span>
            <span
              class="inline-block h-14 w-14 rounded-full -ml-8 bg-[#F202F2]"
            ></span>
          </li>
          <li>
            Hobbies / 🎮 🏋️‍♀️ 🏃‍♂️ ⚽️ 📚
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: "About",
  data() {
    return {
      publicPath: process.env.BASE_URL,
    };
  },
};
</script>
