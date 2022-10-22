<template>
	<div class="container grid grid-col-1 px-16 gap-y-48">
		<div class="flex flex-col gap-y-20">
			<div 
				data-aos="fade-up"
				data-aos-offset="-300"
				data-aos-anchor-placement="center-center"
			>
				<h2
					class="font-univia text-40 text-gray-dark leading-tight capitalize md:text-center"
				>
					More Projects
				</h2>
			</div>
			<p class="font-roboto font-400 text-gray-default mt-32 text-14">
				Some projects that Charlie has been working on the side. You can click
				on the project to learn more or preview a demo.
			</p>
		</div>
		<div class="grid grid-cols-1 md:grid-cols-3 gap-16">
				<div>
				<div class="relative w-full pb-[56.25%] overflow-hidden rounded">
					<a
						href="https://tic-tac-toe-six-pink.vercel.app/"
						target="_blank"
						rel="noopener noreferrer"
						class="group"
					>
						<img
							:src="`${publicPath}img/ticTacToe.gif`"
							:srcset="`${publicPath}img/ticTacToe.gif`"
							class="w-full h-full absolute object-cover group-hover:scale-110 transition-scale duration-200"
							alt=""
						/>
						<span
							class="bg-grape text-white font-roboto bg-grape rounded absolute top-16 right-16 py-4 px-16"
						>
							React + Liveblocks
						</span>
					</a>
				</div>
				<p class="font-roboto font-400 text-gray-default mt-32 text-14">
					A Tic Tac Toe game built with React and Liveblocks. The Liveblocks integrations allows 
					a multiplayer experience and therefore a live state of the game itself. Added UX queues so 
					players can tell if another player is wihtin session. 
				</p>
			</div>
			<div>
				<div class="relative w-full pb-[56.25%] overflow-hidden rounded">
					<a
						href="https://rent-estimate.vercel.app/"
						target="_blank"
						rel="noopener noreferrer"
						class="group"
					>
						<img
							:src="`${publicPath}img/rentEstimate.gif`"
							:srcset="`${publicPath}img/rentEstimate.gif`"
							class="w-full h-full absolute object-cover group-hover:scale-110 transition-scale duration-200"
							alt="snow shader project in unity"
						/>
						<span
							class="bg-grape text-white font-roboto bg-grape rounded absolute top-16 right-16 py-4 px-16"
						>
							React + RestAPI
						</span>
					</a>
				</div>
				<p class="font-roboto font-400 text-gray-default mt-32 text-14">
					A rent estimate app that returns the 5 best matches based on your address search criteria. 
					The app fetches data from <a href="https://rapidapi.com/moneals/api/rent-estimate">Rent Estimate RapidAPI</a>.
				</p>
			</div>
			<div>
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
				<p class="font-roboto font-400 text-gray-default mt-32 text-14">
					EscapeRoomVR is a game built in Unity with SteamVR.
					The main goal is to collect all the tokens hidden before you run out of time.
					The game provides features such as: navigation, interaction to collect tokens and move items
					like doors or chairs, tracks your token collection progress.
				</p>
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
