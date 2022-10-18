<template>
	<div class="container grid grid-col-1 px-16 gap-y-48">
		<div class="flex flex-col gap-y-20">
			<h2
				class="font-univia text-40 text-gray-dark leading-tight capitalize md:text-center"
			>
				Side Projects
			</h2>
			<p class="font-roboto font-400 text-gray-default mt-32 text-14">
				Some projects that Charlie has been working on the side. You can click
				on the project to learn more or preview a demo.
			</p>
		</div>
		<div class="grid grid-cols-1 md:grid-cols-3 gap-16">
			<div class="relative w-full pb-[56.25%] overflow-hidden rounded">
				<a
					href="https://youtu.be/xFZ6y8MjejY"
					target="_blank"
					rel="noopener noreferrer"
					class="group"
				>
					<img
						:src="`${publicPath}img/velocux.png`"
						:srcset="`${publicPath}img/velocux.png`"
						class="w-full h-full absolute object-cover group-hover:scale-110 transition-scale duration-200"
						alt="velocux vr project"
					/>
					<span
						class="bg-grape text-white font-roboto bg-grape rounded absolute top-16 right-16 py-4 px-16"
					>
						VR
					</span>
				</a>
			</div>
			<div class="relative w-full pb-[56.25%] overflow-hidden rounded">
				<a
					href="https://youtu.be/ngwBVBKRnEE"
					target="_blank"
					rel="noopener noreferrer"
					class="group"
				>
					<img
						:src="`${publicPath}img/snow-shaders.png`"
						:srcset="`${publicPath}img/snow-shaders.png`"
						class="w-full h-full absolute object-cover group-hover:scale-110 transition-scale duration-200"
						alt="snow shader project in unity"
					/>
					<span
						class="bg-grape text-white font-roboto bg-grape rounded absolute top-16 right-16 py-4 px-16"
					>
						Unity
					</span>
				</a>
			</div>
			<div class="relative w-full pb-[56.25%] overflow-hidden rounded">
				<a
					href="https://www.fvfesports.org/"
					target="_blank"
					rel="noopener noreferrer"
					class="group"
				>
					<img
						:src="`${publicPath}img/fvfesport.png`"
						:srcset="`${publicPath}img/fvfesport.png`"
						class="w-full h-full absolute object-cover group-hover:scale-110 transition-scale duration-200"
						alt=""
					/>
					<span
						class="bg-grape text-white font-roboto bg-grape rounded absolute top-16 right-16 py-4 px-16"
					>
						Web
					</span>
				</a>
			</div>
		</div>
	</div>
</template>
<script>
export default {
	name: "SideProjects",
	data() {
		return {
			publicPath: process.env.BASE_URL,
		};
	},
	mounted() {
	},
};
</script>
