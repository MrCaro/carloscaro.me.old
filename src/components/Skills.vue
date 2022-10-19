<template>
	<section id="skills" class="">
		<div class="relative container grid grid-col-1 h-full px-16 gap-y-48">
			<div class="flex flex-col gap-y-20">
				<div 
					data-aos="fade-up"
					data-aos-offset="-300"
					data-aos-anchor-placement="center-center"
				>
					<h2
						class="font-univia text-center text-40 text-gray-dark leading-tight"
					>
						Technical
						<span class="title--gradient">
							Skills
						</span>
					</h2>
				</div>
				<!-- <p class="font-roboto font-400 text-gray-default text-14 mt-32">
					For specifics you can refer to highlighted projects and check the tech
					stack.
				</p> -->
			</div>
			<div class="flex flex-wrap gap-32 md:gap-88 mt-32">
				<div class="">
					<p class="font-univia text-14 text-gray-dark leading-tight">
						Dev
					</p>
					<ul class="flex font-roboto font-400 text-gray-default text-12 mt-4">
						<li class="mr-16">React</li>
						<li class="mr-16">Shopify</li>
						<li class="mr-16">TailwindCSS</li>
						<li class="mr-16">Twig</li>
						<li class="mr-16">Vue</li>
						<li class="mr-16">WordPress</li>
					</ul>
				</div>
				<div class="">
					<p class="font-univia text-14 text-gray-dark leading-tight">
						UI Design
					</p>
					<ul class="flex font-roboto font-400 text-gray-default text-12 mt-4">
						<li class="mr-16">Adobe XD</li>
						<li class="mr-16">Figma</li>
					</ul>
				</div>
				<div>
					<p class="font-univia text-14 text-gray-dark leading-tight">
						VR
					</p>
					<ul class="flex font-roboto font-400 text-gray-default text-12 mt-4">
						<li class="mr-16">SteamVR</li>
						<li class="mr-16">Unity</li>
					</ul>
				</div>
				<div>
					<p class="font-univia text-14 text-gray-dark leading-tight">
						AR
					</p>
					<ul class="flex font-roboto font-400 text-gray-default text-12 mt-4">
						<li class="mr-16">Unity</li>
						<li class="mr-16">Vuforia</li>
					</ul>
				</div>
				<div>
					<p class="font-univia text-14 text-gray-dark leading-tight">
						Other
					</p>
					<ul class="flex font-roboto font-400 text-gray-default text-12 mt-4">
						<li class="mr-16">Git</li>
						<li class="mr-16">Notion</li>
					</ul>
				</div>
			</div>
			<div class="relative h-[148px] lg:h-[332px] mt-128">
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
