<template>
  <section class="test relative bg-gray-light pt-52 pb-60">
    <img
      :src="`${publicPath}img/gradient-noise.jpeg`"
      :srcset="`${publicPath}img/gradient-noise.jpeg`"
      class="absolute bottom-0 h-full w-full"
      alt=""
    />
    <div
      class="relative container grid grid-col-1 md:grid-cols-2 h-full px-16 gap-y-48"
    >
      <div class="flex flex-col justify-center">
        <h1 class="font-univia text-60 text-gray-dark leading-tight">
          <span class="inline-block hero--title-top">
            Front-End
          </span>
          <br />
          <span
            class="text-gray-light inline-block hero--title-bottom mix-blend-color-burn"
            style="text-shadow: -1px -1px 0 #b928e5, 1px -1px 0 #b928e5, -1px 1px 0 #b928e5, 1px 1px 0 #b928e5;"
          >
            Developer.
          </span>
        </h1>
        <p class="font-roboto font-400 text-gray-default my-20">
          Crafting digital experiences one key stroke at a time.
        </p>
        <p class="font-roboto font-400 text-gray-default text-12 m-0">
          📍 Orlando, FL <br />
          💻 Web Developer at Tasty Studio
        </p>
      </div>
      <div class="relative flex flex-col items-center justify-center">
        <div class="relative">
          <img
            :src="`${publicPath}icons/squaredot-pattern.svg`"
            :srcset="`${publicPath}icons/squaredot-pattern.svg`"
            alt=""
            class="absolute top-[-2rem] right-[-4rem]"
          />
          <img
            :src="`${publicPath}icons/squaredot-pattern.svg`"
            :srcset="`${publicPath}icons/squaredot-pattern.svg`"
            alt=""
            class="absolute bottom-[-1rem] left-[-3rem] "
          />
          <img
            :src="`${publicPath}img/hero-banner-computer@2x.png`"
            :srcset="`${publicPath}img/hero-banner-computer@2x.png`"
            alt="Charlie headshot"
            class="hero--img relative h-[372px] w-auto z-1"
            style="filter: drop-shadow(11px 11px 10px #00000029);"
          />
          <div
            id="GlassBox1"
            class="group absolute left-[-3rem] top-[9rem] flex justify-center items-center rounded-xl bg-white cursor-pointer"
            style="box-shadow: 0 0 5rem 0 rgba(0, 0, 0, .3)"
            @click="setIsOpen(true), (playing = !playing)"
          >
            <div
              class="relative h-auto w-auto flex items-center gap-16 rounded-xl transition-transform ease-out duration-200 delay-200 group-hover:scale-75"
            >
              <div>
                <svg
                  viewBox="0 0 24 24"
                  xmlns="http://www.w3.org/2000/svg"
                  width="80"
                  height="80"
                  fill="none"
                >
                  <circle
                    cx="12"
                    cy="12"
                    r="6"
                    fill="#b928e5"
                    style="animation:loader15 1.5s cubic-bezier(.165,.84,.44,1) infinite both;transform-origin:center center"
                  />
                  <path
                    fill="#b928e5"
                    fill-rule="evenodd"
                    d="M13.41 11.591a.5.5 0 010 .817l-1.73 1.222a.5.5 0 01-.788-.409v-2.442a.5.5 0 01.789-.409l1.729 1.222z"
                    clip-rule="evenodd"
                  />
                </svg>
              </div>
            </div>
          </div>
          <div
            class="absolute right-[2rem] bottom-[-1rem] flex justify-center items-center"
          >
            <div
              class="absolute h-full w-full filter rounded-xl bg-white"
              style="box-shadow: 0 0 5rem 0 rgba(0, 0, 0, .3)"
            ></div>
            <div class="group relative h-auto w-auto px-20 py-12">
              <p
                class="text-28 transition-transform ease-in duration-200 delay-200 group-hover:rotate-12"
              >
                👋
              </p>
            </div>
          </div>
        </div>
      </div>
      <div
        class="absolute h-192 border-l-2 border-gray-[#848b9e] right-0 md:right-[unset] bottom-0 md:left-0 mr-60 md:mr-0 mb-[-180px] md:ml-160"
      ></div>
    </div>
    <Dialog class="relative z-[20]" :open="isOpen" :unmount="false">
      <DialogOverlay class="fixed inset-0 bg-black opacity-30 z-[-1]" />
      <div class="fixed inset-0 flex items-center justify-center p-4">
        <DialogPanel
          class="flex flex-col gap-8 w-[fit-content] h-[fit-content] bg-white py-32 px-32 md:px-64 rounded w-[80vw] md:w-[800px]"
        >
          <DialogTitle
            class="font-roboto font-400 text-gray-default text-center"
          >
            Hello there stranger and welcome 👋
          </DialogTitle>
          <DialogDescription>
            <video class="plyr-intro h-auto rounded">
              <source
                src="https://res.cloudinary.com/dbyzfcnpg/video/upload/v1652491432/charlie_intro_lbccau.mp4"
                type="video/mp4"
              />
            </video>
          </DialogDescription>
          <button
            class="bg-grape rounded p-6 text-14 text-white font-roboto font-700 capitalize border-2 border-grape transition duration-500 ease-in-out hover:scale-105 hover:bg-white hover:text-grape"
            @click="setIsOpen(false), (playing = !playing)"
          >
            close modal
          </button>
        </DialogPanel>
      </div>
    </Dialog>
  </section>
</template>

<script type="text/javascript">
import {
  Dialog,
  DialogPanel,
  DialogOverlay,
  DialogTitle,
  DialogDescription,
} from "@headlessui/vue";
import Plyr from "plyr";
import "plyr/dist/plyr.css";

export default {
  name: "MainHero",
  components: {
    Dialog,
    DialogPanel,
    DialogOverlay,
    DialogTitle,
    DialogDescription,
  },
  data() {
    return {
      publicPath: process.env.BASE_URL,
      isOpen: false,
      plyr: null,
      playing: false,
    };
  },
  mounted() {
    this.plyr = document.querySelector(".plyr-intro");
    new Plyr(this.plyr, {
      autoplay: false,
      iconPrefix: "plyr",
    });
  },
  watch: {
    playing: function(value) {
      console.log(value);
      if (value) {
        this.plyr.play();
        this.plyr.volume = 1;
      } else {
        this.plyr.pause();
      }
    },
  },
  methods: {
    setIsOpen: function(value) {
      this.isOpen = value;
    },
  },
};
</script>
