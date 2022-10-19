<template>
	<div id="app">
		<NavBar />
		<main class="grid gap-y-96 md:gap-y-192 overflow-x-hidden relative z-0">
			<MainHero />
			<About />
			<Work />
			<SideProjects />
			<Skills />
			<Collab />
			<Wall />
			<Footer />
		</main>
		<!-- <cursor-fx  /> -->
		<div class="invisible md:visible">
			<custom-cursor
				:targets="['img', 'a', 'button', 'your-hover-class']"
				:circleColor="'#b928e5'"
				:circleColorHover="'#2f2f2f'"
				:dotColor="'#b928e5'"
				:dotColorHover="'#2f2f2f'"
				:hoverSize="1.8"
			></custom-cursor>
		</div>
	</div>
</template>

<script type="text/javascript">
import AOS from 'aos';
import 'aos/dist/aos.css'; 
import gsap from "gsap";
import ScrollTrigger from "gsap/ScrollTrigger";

import About from "@/components/About.vue";
import CustomCursor from "@/components/CustomCursor.vue";
import Collab from "@/components/Collab.vue";
import Footer from "@/components/Footer.vue";
import MainHero from "@/components/MainHero.vue";
import NavBar from "@/components/NavBar.vue";
import SideProjects from "@/sections/SideProjects.vue";
import Skills from "@/components/Skills.vue";
import Wall from "@/components/Wall.vue";
import Work from "@/components/Work.vue";

gsap.registerPlugin(ScrollTrigger);

export default {
	components: {
		// 'cursor-fx': CursorFx,
		About,
		CustomCursor,
		Collab,
		MainHero,
		NavBar,
		SideProjects,
		Skills,
		Footer,
		Wall,
		Work,
	},
	mounted: function() {
		AOS.init();
		//hero
		ScrollTrigger.matchMedia({
			"(min-width: 0px)": function() {
				gsap.to(document.querySelector(".hero--img"), {
					scrollTrigger: {
						trigger: ".hero--img",
						start: "top",
						end: "bottom center",
						scrub: 2,
						// markers: true,
					},
					y: 20,
					duration: 3,
				});
			},
		});
		ScrollTrigger.matchMedia({
			"(min-width: 768px)": function() {
				gsap.to(document.querySelector(".hero--title-top"), {
					scrollTrigger: {
						trigger: ".hero--img",
						start: "top",
						end: "bottom center",
						scrub: 2,
					},
					x: 60,
					duration: 4,
				});
			},
		});
		ScrollTrigger.matchMedia({
			"(min-width: 768px)": function() {
				gsap.to(document.querySelector(".hero--title-bottom"), {
					scrollTrigger: {
						trigger: ".hero--img",
						start: "top",
						end: "bottom center",
						scrub: 2,
					},
					x: -60,
					duration: 4,
				});
			},
		});
		//about
		ScrollTrigger.matchMedia({
			"(min-width: 0px)": function() {
				gsap.to(document.querySelector(".headshot"), {
					scrollTrigger: {
						trigger: ".headshot",
						start: "top center",
						end: "bottom center",
						scrub: 2,
						// markers: true,
					},
					y: 50,
					duration: 3,
				});
			},
		});
	},
};
</script>
