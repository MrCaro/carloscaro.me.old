<template>
  <div id="app">
    <NavBar />
    <main class="grid gap-y-96 md:gap-y-192">
      <MainHero />
      <About />
      <Work />
      <Skills />
      <Collab />
      <Footer />
    </main>
    <!-- <cursor-fx  /> -->
    <custom-cursor
      :targets="['img', 'a', 'button', 'your-hover-class']"
      :circleColor="'#b928e5'"
      :circleColorHover="'#2f2f2f'"
      :dotColor="'#b928e5'"
      :dotColorHover="'#2f2f2f'"
      :hoverSize="1.8"
    ></custom-cursor>
  </div>
</template>

<script type="text/javascript">
// import { CursorFx } from '@luxdamore/vue-cursor-fx';
import gsap  from "gsap";
import ScrollTrigger from "gsap/ScrollTrigger";
gsap.registerPlugin(ScrollTrigger);

import NavBar from "@/components/NavBar.vue";
import MainHero from "@/components/MainHero.vue";
import About from "@/components/About.vue";
import Work from "@/components/Work.vue";
import Skills from "@/components/Skills.vue";
import Collab from "@/components/Collab.vue";
import Footer from "@/components/Footer.vue";
import CustomCursor from "@/components/CustomCursor.vue";



export default {
  components: {
    // 'cursor-fx': CursorFx,
    NavBar,
    MainHero,
    About,
    Work,
    Skills,
    Collab,
    Footer,
    CustomCursor
  },
  mounted: function(){
        //glass boxes
        let glass1 = document.querySelector('#GlassBox1');
        ScrollTrigger.matchMedia({
          "(max-width: 768px)": function() {
            gsap.to(glass1,{
              scrollTrigger: {
                  trigger: "#GlassBox1",
                  start: "top center",
                  end: "bottom center",
                  scrub: 2,
                  // markers: true,
              },
              x: '100%', 
              duration: 3,
            })}
        })
        //headshots 
        let headshots = document.getElementsByClassName('headshot');
        console.log(headshots)
        let images = [].map.call(headshots, headshot => {
          gsap.to(headshot, 
              {
                  scrollTrigger: {
                      trigger: ".headshot",
                      start: "top center",
                      end: "bottom center",
                      scrub: 2,
                      // markers: true,
                  },
                  y: 50, 
                  duration: 3,
              })
        });
        console.log(images)
    }
};
</script>