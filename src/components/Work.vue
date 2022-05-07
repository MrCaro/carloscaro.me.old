<template>
  <section id="work" class="">
    <div class="container grid grid-col-1 h-full px-16">
      <div class="flex flex-col gap-y-20">
        <h2
          class="font-univia text-40 text-gray-dark leading-tight capitalize md:text-center"
        >
          charlie's recent
          <span
            class="text-white"
            style="text-shadow: -1px -1px 0 #b928e5, 1px -1px 0 #b928e5, -1px 1px 0 #b928e5, 1px 1px 0 #b928e5;"
          >
            Work
          </span>
          on the web
        </h2>
        <!-- bardega cocktails -->
        <h3
          class="font-univia text-30 text-gray-dark leading-tight capitalize text-left mt-64 md:-ml-64"
        >
          bardega cocktails
        </h3>
        <div class="grid grid-col-1 md:grid-cols-2 gap-32 md:gap-16">
          <div class="flex flex-col">
            <p class="font-roboto font-400 text-14 text-gray-default m-0">
              Led this custom e-commerce web project from development
              perspective. Assisted client to transition from wocommerce store
              to Shopify, which involved plugin integrations to match current
              and exhance features requested from client. Also, I was
              responsible for new website redesign (dev).
            </p>
            <p class="font-roboto font-400 text-14 text-gray-default mt-12">
              <strong>Features</strong>
            </p>
            <ul class="font-roboto font-400 text-14 text-gray-default m-0">
              <li>
                Subscription based e-commerce.
              </li>
              <li>
                Custom blocks and templates creation for client to easily
                edit/maintain the online store.
              </li>
            </ul>
            <p class="font-roboto font-400 text-14 text-gray-default mt-12">
              <strong>Tech Stack</strong>
            </p>
            <ul class="font-roboto font-400 text-14 text-gray-default m-0">
              <li>
                Shopify / Liquid
              </li>
            </ul>
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
                <vs-avatar
                  size="medium"
                  src="https://avatars2.githubusercontent.com/u/36524539?s=460&v=4"
                />
              </a>
            </div>
            <div class="flex mt-24">
              <MainCTA
                url="https://bardegacocktails.com/"
                title="checkout bardega cocktails 🍹"
              />
            </div>
          </div>
          <div>
            <a
              href="https://bardegacocktails.com/"
              target="_blank"
              rel="noopener noreferrer"
            >
              <img
                :src="`${publicPath}img/bardega-cocktails-poster.png`"
                :srcset="`${publicPath}img/bardega-cocktails-poster.png`"
                alt="Bardega Cocktails"
              />
            </a>
            <!-- <video
              class="video-plyr-component w-full h-full"
              src="https://res.cloudinary.com/dbyzfcnpg/video/upload/v1648336568/vr_escape_room.mp4"
              :poster="`${publicPath}img/vr-escape-room-poster.jpg`"
            ></video> -->
          </div>
        </div>
        <!-- vr escape room -->
        <h3
          class="font-univia text-30 text-gray-dark leading-tight capitalize text-left mt-64 md:-ml-64"
        >
          VR escape room
        </h3>
        <div class="grid grid-col-1 md:grid-cols-2 gap-32 md:gap-16">
          <div class="flex flex-col md:order-2">
            <p class="font-roboto font-400 text-14 text-gray-default m-0">
              Recreate a digital escape room experience while using a VR headset
              to stimulate user's critical thinking and problem solving. Players
              will be presented with a list of clues as a hint where the tokens
              that they need to collect are hidden within the virtual room. They
              have to collect these tokens within a time constrain to make it
              more challenging.
            </p>
            <p class="font-roboto font-400 text-14 text-gray-default mt-12">
              <strong>Features</strong>
            </p>
            <ul class="font-roboto font-400 text-14 text-gray-default m-0">
              <li>
                Game state based on clues collected and state of timer.
              </li>
              <li>
                Clues are removed from the main list once associated token is
                collected by player.
              </li>
            </ul>
            <p class="font-roboto font-400 text-14 text-gray-default mt-12">
              <strong>Tech Stack</strong>
            </p>
            <ul class="font-roboto font-400 text-14 text-gray-default m-0">
              <li>
                Unity / SteamVR / Oculus Quest 2
              </li>
            </ul>
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
                <vs-avatar
                  size="medium"
                  src="https://avatars2.githubusercontent.com/u/36524539?s=460&v=4"
                />
              </a>
            </div>
          </div>
          <div>
            <video
              class="video-plyr-component w-full h-full"
              src="https://res.cloudinary.com/dbyzfcnpg/video/upload/v1648336568/vr_escape_room.mp4"
              :poster="`${publicPath}img/vr-escape-room-poster.jpg`"
            ></video>
          </div>
        </div>
        <!-- snow shader -->
        <h3
          class="font-univia text-30 text-gray-dark leading-tight capitalize text-left mt-64 md:-ml-64"
        >
          snow shader
        </h3>
        <div class="grid grid-col-1 md:grid-cols-2 gap-32 md:gap-16">
          <div class="flex flex-col">
            <p class="font-roboto font-400 text-14 text-gray-default m-0">
              The components for simulating snow consist of snowflake,
              environment properties (temperature, wind, light, dust, gravity,
              etc.) and surface properties (occluder, surface slope, surface
              material, etc.). For this particular project I foused on wind.
            </p>
            <p class="font-roboto font-400 text-14 text-gray-default mt-12">
              <strong>Features</strong>
            </p>
            <ul class="font-roboto font-400 text-14 text-gray-default m-0">
              <li>
                You can set direction and strength of snow accumulated on the
                physical object. You can adjust these settings from the Unity
                editor.
              </li>
              <li>
                You can interact with the surface terrain to remove snow based
                on brush stregth and size. You can toggle a canvas view for the
                actual displacement of the brush on the surface.
              </li>
            </ul>
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
                <vs-avatar
                  size="medium"
                  src="https://avatars2.githubusercontent.com/u/36524539?s=460&v=4"
                />
              </a>
            </div>
          </div>
          <div>
            <video
              class="video-plyr-component w-full h-full"
              src="https://res.cloudinary.com/dbyzfcnpg/video/upload/v1642459842/snow_accumulation.mp4"
              :poster="`${publicPath}img/snow-accumulation-poster.jpg`"
            ></video>
          </div>
        </div>
        <!-- <p class="font-roboto font-400 text-gray-default mt-32 text-left">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Saepe eos a excepturi explicabo quidem fuga. Esse quod consequatur non aspernatur maxime et, voluptas nostrum eveniet quo aut dicta ex dolore!
                </p> -->
        <!-- <vs-button color="success" type="flat" icon="visibility">Done</vs-button>
                <vs-button @click="$vs.notify({title:'Default',text:'Lorem ipsum dolor sit amet, consectetur'})" color="primary" type="border">Notification white</vs-button> -->
        <!-- <hr class="my-32"> -->
        <div class="flex md:justify-center items-center gap-x-16 mt-32">
          <vs-button
            class="w-[fit-content]"
            @click="
              $vs.notify({
                title: 'Coming Fall 2022 👀',
                text: 'Description: AR Application </br> Tech: Unity / Vuforia',
                color: '#b928e5',
              })
            "
            color="#b928e5"
            type="border"
            >Upcoming Project AR Laroma</vs-button
          >
        </div>
      </div>
    </div>
  </section>
</template>

<script>
// import Vue from 'vue'
import MainCTA from "@/components/MainCTA.vue";
import Plyr from "plyr";
import "plyr/dist/plyr.css";

export default {
  name: "Work",
  components: {
    MainCTA,
  },
  data() {
    return {
      publicPath: process.env.BASE_URL,
    };
  },
  mounted() {
    document.querySelectorAll(".video-plyr-component").forEach((el) => {
      new Plyr(el, {
        autoplay: false,
        muted: true,
        iconPrefix: "plyr",
        // controls: false
        // iconUrl: '/wp-content/themes/scripps/src/assets/icons/plyr.svg'
      });
    });
  },
};
</script>
