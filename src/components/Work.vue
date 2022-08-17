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
        <div class="container mt-60">
          <TabGroup>
            <div class="grid grid-cols-12">
              <TabList class="col-span-12 lg:col-span-2">
                <div class="grid grid-cols-2 lg:grid-cols-1 gap-20">
                  <!-- bardega -->
                  <Tab v-slot="{ selected }" class="">
                    <button
                      class="w-full text-gray-dark font-roboto font-700 capitalize py-20 px-10 border-2 border-white rounded-[12px] transition duration-500 ease-in-out hover:bg-white hover:border-gray-light flex justify-between items-center"
                      :class="[
                        selected
                          ? 'bg-gray-light hover:bg-gray-light'
                          : 'bg-white',
                      ]"
                    >
                      <span class="text-left">
                        Bardega
                      </span>
                      <span>
                        🍹
                      </span>
                    </button>
                  </Tab>
                  <!-- scripps -->
                  <Tab v-slot="{ selected }" class="">
                    <button
                      class="w-full text-gray-dark font-roboto font-700 capitalize py-20 px-10 border-2 border-white rounded-[12px] transition duration-500 ease-in-out hover:bg-white hover:border-gray-light flex justify-between items-center"
                      :class="[
                        selected
                          ? 'bg-gray-light hover:bg-gray-light'
                          : 'bg-white',
                      ]"
                    >
                      <span class="text-left">
                        SCRIPPS
                      </span>
                      <span>
                        🎓
                      </span>
                    </button>
                  </Tab>
                  <!-- k10 -->
                  <Tab v-slot="{ selected }" class="">
                    <button
                      class="w-full text-gray-dark font-roboto font-700 capitalize py-20 px-10 border-2 border-white rounded-[12px] transition duration-500 ease-in-out hover:bg-white hover:border-gray-light flex justify-between items-center"
                      :class="[
                        selected
                          ? 'bg-gray-light hover:bg-gray-light'
                          : 'bg-white',
                      ]"
                    >
                      <span class="text-left">
                        Keystone 10
                      </span>
                      <span>
                        🌳
                      </span>
                    </button>
                  </Tab>
                  <!-- brp -->
                  <Tab v-slot="{ selected }" class="">
                    <button
                      class="w-full text-gray-dark font-roboto font-700 capitalize py-20 px-10 border-2 border-white rounded-[12px] transition duration-500 ease-in-out hover:bg-white hover:border-gray-light flex justify-between items-center"
                      :class="[
                        selected
                          ? 'bg-gray-light hover:bg-gray-light'
                          : 'bg-white',
                      ]"
                    >
                      <span class="text-left">
                        BRP
                      </span>
                      <span>
                        🎥
                      </span>
                    </button>
                  </Tab>
                </div>
              </TabList>
              <TabPanels
                class="col-span-12 lg:col-start-4 lg:col-span-9 mt-60 lg:mt-0"
              >
                <!-- bardega -->
                <TabPanel class="grid grid-cols-12 gap-32">
                  <img
                    class="col-span-12 w-[150px]"
                    :src="`${publicPath}img/bardega-logo.png`"
                    :srcset="`${publicPath}img/bardega-logo.png`"
                    alt=""
                  />
                  <div class="col-span-12 md:col-span-3">
                    <p class="font-roboto font-600 text-gray-default text-14">
                      Features
                    </p>
                    <ul
                      class="font-roboto font-400 text-gray-default text-12 mt-12"
                    >
                      <li>Subscription based e-commerce.</li>
                      <li class="mt-6">
                        Custom blocks and templates creation for client to
                        easily edit/maintain the online store.
                      </li>
                    </ul>
                    <p
                      class="font-roboto font-600 text-gray-default text-14 mt-20"
                    >
                      Role
                    </p>
                    <p
                      class="font-roboto font-400 text-gray-default text-12 mt-12"
                    >
                      Lead Web Developer
                    </p>
                    <p
                      class="font-roboto font-600 text-gray-default text-14 mt-20"
                    >
                      Tech Stack
                    </p>
                    <p
                      class="font-roboto font-400 text-gray-default text-12 mt-12"
                    >
                      Shopify Liquid
                    </p>
                    <p
                      class="font-roboto font-600 text-gray-default text-14 mt-20"
                    >
                      Visit
                    </p>
                    <a
                      class="font-roboto font-400 text-grape text-12 mt-12"
                      href="https://bardegacocktails.com/"
                      target="_blank"
                      rel="noopener noreferrer"
                    >
                      click to view project
                    </a>
                  </div>
                  <div class="col-span-12 md:col-start-4 md:col-span-9">
                    <p class="font-roboto font-400 text-gray-default text-14">
                      Charlie led this custom e-commerce web project from
                      development perspective. He assisted Bardega to transition
                      from wocommerce to Shopify, which involved plugin
                      integrations to match current and exhance features
                      requested from client. Also, Charlie was responsible for
                      coding the new website redesign.
                    </p>
                    <p
                      class="font-roboto font-600 text-gray-default text-14 mt-20"
                    >
                      Challenges
                    </p>
                    <ul
                      class="font-roboto font-400 text-gray-default text-14 mt-12"
                    >
                      <li>
                        While deving the project Charlie managed the integration
                        to offer different subscription options to customers
                        while creating a user portal. Discovered segmentation
                        between product and services to allow a better UX
                        mapping of the e-commerce site. Final outcome, a fully
                        functional user portal that manages accurately user
                        subscriptions.
                      </li>
                      <li class="mt-6">
                        Creating reusable yaml files for components across the
                        site. The client requested to reuse sections/components
                        across the site, so it was paramount to accomplish this
                        feature. Charlie created resuable components by
                        registering them in liquid functions and pass unique ids
                        to allow reuse. End result, client was able to reuse
                        section across different templates within the site.
                      </li>
                    </ul>
                  </div>
                </TabPanel>
                <!-- scripps -->
                <TabPanel class="grid grid-cols-12 gap-32">
                  <img
                    class="col-span-12 w-[150px]"
                    :src="`${publicPath}img/scripps-logo.svg`"
                    :srcset="`${publicPath}img/scripps-logo.svg`"
                    alt=""
                  />
                  <div class="col-span-12 md:col-span-3">
                    <p class="font-roboto font-600 text-gray-default text-14">
                      Features
                    </p>
                    <ul
                      class="font-roboto font-400 text-gray-default text-12 mt-12"
                    >
                      <li>
                        Custom animations when scrolling through the site.
                      </li>
                      <li class="mt-6">
                        Carousel + a filter feature.
                      </li>
                    </ul>
                    <p
                      class="font-roboto font-600 text-gray-default text-14 mt-20"
                    >
                      Role
                    </p>
                    <p
                      class="font-roboto font-400 text-gray-default text-12 mt-12"
                    >
                      Lead Web Developer
                    </p>
                    <p
                      class="font-roboto font-600 text-gray-default text-14 mt-20"
                    >
                      Tech Stack
                    </p>
                    <p
                      class="font-roboto font-400 text-gray-default text-12 mt-12"
                    >
                      Twig / VueJS / TailwindCSS / WordPress
                    </p>
                    <p
                      class="font-roboto font-600 text-gray-default text-14 mt-20"
                    >
                      Visit
                    </p>
                    <a
                      class="font-roboto font-400 text-grape text-12 mt-12"
                      href="https://explore.scrippscollege.edu/"
                      target="_blank"
                      rel="noopener noreferrer"
                    >
                      click to view project
                    </a>
                  </div>
                  <div class="col-span-12 md:col-start-4 md:col-span-9">
                    <p class="font-roboto font-400 text-gray-default text-14">
                      Charlie led this custom microsite for SCRIPPS College.
                    </p>
                    <p
                      class="font-roboto font-600 text-gray-default text-14 mt-20"
                    >
                      Challenges
                    </p>
                    <ul
                      class="font-roboto font-400 text-gray-default text-14 mt-12"
                    >
                      <li>
                        This specific project involved a lot of customization
                        and interactions within components. For the activity
                        section (carousel) Charlie had to combine a slider + a
                        filter option, so future stundets can search through
                        them based on their own preferences. Charlie managed the
                        state of the swipper carousel with vue states. At the
                        end, we have a carousel with a functional filter.
                      </li>
                    </ul>
                  </div>
                </TabPanel>
                <!-- k10 -->
                <TabPanel class="grid grid-cols-12 gap-32">
                  <img
                    class="col-span-12 w-[150px]"
                    :src="`${publicPath}img/k10-logo.png`"
                    :srcset="`${publicPath}img/k10-logo.png`"
                    alt=""
                  />
                  <div class="col-span-12 md:col-span-3">
                    <p class="font-roboto font-600 text-gray-default text-14">
                      Features
                    </p>
                    <ul
                      class="font-roboto font-400 text-gray-default text-12 mt-12"
                    >
                      <li>Tree Counter</li>
                      <li class="mt-6">
                        Display content based on user's location (PA County)
                      </li>
                      <li class="mt-6">
                        Partner user role to create content within the site.
                      </li>
                    </ul>
                    <p
                      class="font-roboto font-600 text-gray-default text-14 mt-20"
                    >
                      Role
                    </p>
                    <p
                      class="font-roboto font-400 text-gray-default text-12 mt-12"
                    >
                      Lead Front-End Web Developer
                    </p>
                    <p
                      class="font-roboto font-600 text-gray-default text-14 mt-20"
                    >
                      Tech Stack
                    </p>
                    <p
                      class="font-roboto font-400 text-gray-default text-12 mt-12"
                    >
                      Twig / VueJS / TailwindCSS / WordPress
                    </p>
                    <p
                      class="font-roboto font-600 text-gray-default text-14 mt-20"
                    >
                      Visit
                    </p>
                    <a
                      class="font-roboto font-400 text-grape text-12 mt-12"
                      href="http://tenmilliontrees.org/"
                      target="_blank"
                      rel="noopener noreferrer"
                    >
                      click to view project
                    </a>
                  </div>
                  <div class="col-span-12 md:col-start-4 md:col-span-9">
                    <p class="font-roboto font-400 text-gray-default text-14">
                      Charlie led this custom site for Keystone 10 marketing
                      efforts to plan 10M trees by 2025. Project was a redesign
                      and also an enhacement of current website
                    </p>
                    <p
                      class="font-roboto font-600 text-gray-default text-14 mt-20"
                    >
                      Challenges
                    </p>
                    <ul
                      class="font-roboto font-400 text-gray-default text-14 mt-12"
                    >
                      <li>
                        video + audio modals
                      </li>
                      <li class="mt-6">
                        partner role
                      </li>
                      <li class="mt-6">
                        contact pages ids
                      </li>
                      <li class="mt-6">
                        tree animation
                      </li>
                      <li class="mt-6">
                        map out sections / naming of components
                      </li>
                    </ul>
                  </div>
                </TabPanel>
                <!-- brp -->
                <TabPanel class="grid grid-cols-12 gap-32">
                  <img
                    class="col-span-12 w-[150px]"
                    :src="`${publicPath}img/brp-logo.svg`"
                    :srcset="`${publicPath}img/brp-logo.svg`"
                    alt=""
                  />
                  <div class="col-span-12 md:col-span-3">
                    <p class="font-roboto font-600 text-gray-default text-14">
                      Features
                    </p>
                    <ul
                      class="font-roboto font-400 text-gray-default text-12 mt-12"
                    >
                      <li>n/a</li>
                    </ul>
                    <p
                      class="font-roboto font-600 text-gray-default text-14 mt-20"
                    >
                      Role
                    </p>
                    <p
                      class="font-roboto font-400 text-gray-default text-12 mt-12"
                    >
                      Lead Front-End Web Developer
                    </p>
                    <p
                      class="font-roboto font-600 text-gray-default text-14 mt-20"
                    >
                      Tech Stack
                    </p>
                    <p
                      class="font-roboto font-400 text-gray-default text-12 mt-12"
                    >
                      Twig / VueJS / TailwindCSS / WordPress
                    </p>
                    <p
                      class="font-roboto font-600 text-gray-default text-14 mt-20"
                    >
                      Visit
                    </p>
                    <a
                      class="font-roboto font-400 text-grape text-12 mt-12"
                      href="https://brpentertainment.com"
                      target="_blank"
                      rel="noopener noreferrer"
                    >
                      click to view project
                    </a>
                  </div>
                  <div class="col-span-12 md:col-start-4 md:col-span-9">
                    <p class="font-roboto font-400 text-gray-default text-14">
                      Charlie led this web project from start to finish. Client
                      was looking for a complete website redesign.
                    </p>
                  </div>
                </TabPanel>
              </TabPanels>
            </div>
          </TabGroup>
        </div>
        <!-- <div class="flex md:justify-center items-center gap-x-16 mt-32">
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
        </div> -->
      </div>
    </div>
  </section>
</template>

<script>
// import Vue from 'vue'
import { TabGroup, TabList, Tab, TabPanels, TabPanel } from "@headlessui/vue";
// import MainCTA from "@/components/MainCTA.vue";
// import Plyr from "plyr";
import "plyr/dist/plyr.css";

export default {
  name: "Work",
  components: {
    TabGroup,
    TabList,
    Tab,
    TabPanels,
    TabPanel,
  },
  data() {
    return {
      publicPath: process.env.BASE_URL,
    };
  },
  mounted() {
    // document.querySelectorAll(".video-plyr-component").forEach((el) => {
    //   new Plyr(el, {
    //     autoplay: false,
    //     muted: true,
    //     iconPrefix: "plyr",
    //     // controls: false
    //     // iconUrl: '/wp-content/themes/scripps/src/assets/icons/plyr.svg'
    //   });
    // });
  },
};
</script>
