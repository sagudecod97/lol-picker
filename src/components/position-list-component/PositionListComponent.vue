<template>
	<div class="position-list">
		<div class="position-list__header">
			<img
				class="position-list__img"
				v-if="rol === 'top'"
				src="../../assets/Position_Gold-Top.png"
				alt=""
			/>

			<img
				class="position-list__img"
				v-if="rol === 'jungle'"
				src="../../assets/Position_Gold-Jungle.png"
				alt=""
			/>

			<img
				class="position-list__img"
				v-if="rol === 'mid'"
				src="../../assets/Position_Gold-Mid.png"
				alt=""
			/>

			<img
				class="position-list__img"
				v-if="rol === 'adc'"
				src="../../assets/Position_Gold-Bot.png"
				alt=""
			/>

			<img
				class="position-list__img"
				v-if="rol === 'supp'"
				src="../../assets/Position_Gold-Support.png"
				alt=""
			/>

			<svg
				class="position-list__icon"
				xmlns="http://www.w3.org/2000/svg"
				viewBox="0 0 20 20"
				fill="currentColor"
			>
				<path
					fill-rule="evenodd"
					d="M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z"
					clip-rule="evenodd"
				/>
			</svg>

			<hr class="position-list__header-separator" />
		</div>

		<div class="position-list__container">
			<div class="player" v-for="player in positionList" :key="player.id">
				<p class="player__name">{{ player.playerName }}</p>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "PositionListComponent",
	props: {
		rol: {
			type: String,
			required: true,
		},
		positionList: {
			type: Array,
			required: true,
		},
	},
};
</script>

<style scoped>
.position-list {
	border: 3px solid goldenrod;
	width: 100%;
	max-width: 250px;
	height: 100%;
	background: #0d2c54;
	box-shadow: 0px 0px 5px black;
	position: relative;
}

.position-list__header {
	height: 22%;
	display: flex;
	justify-content: center;
	padding: 10px;
	position: relative;
}

.position-list__img {
	height: 100%;
}

.position-list__icon {
	color: #deb841;
	height: 25px;
	width: 25px;
	justify-self: flex-end;
	position: absolute;
	right: 10px;
	top: 50%;
	transform: translateY(-50%);
	cursor: pointer;
}

.position-list__header-separator {
	position: absolute;
	bottom: 0;
	width: 95%;
	height: 2px;
	background-color: #deb841;
	border: none;
}

.position-list__container {
	height: 78%;
	width: 95%;
	display: flex;
	flex-direction: column;
	padding: 4px 0;
	margin: 0 auto;
	gap: 2px;
	overflow-y: auto;
}

.player {
	border: 1px solid #deb841;
	padding: 5px;
}

.player__name {
	text-align: center;
	color: #deb841;
	font-size: 16px;
}
</style>
