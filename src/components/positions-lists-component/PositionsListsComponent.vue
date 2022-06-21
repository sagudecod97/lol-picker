<template>
	<div class="positions-lists">
		<position-list-component :rol="'top'" :position-list="playersTop" />
		<position-list-component :rol="'jungle'" :position-list="playerJungle" />
		<position-list-component :rol="'mid'" :position-list="playersMid" />
		<position-list-component :rol="'adc'" :position-list="playersAdc" />
		<position-list-component :rol="'supp'" :position-list="playersSupp" />
	</div>
</template>

<script>
import PositionListComponent from "../position-list-component/PositionListComponent.vue";

export default {
	name: "PositionsListsComponent",
	data() {
		return {
			playersTop: [
				{ playerName: "SirNagi", id: 1 },
				{ playerName: "Aborig3N", id: 2 },
				{ playerName: "CarlosRC22", id: 3 },
			],
			playerJungle: [
				{ playerName: "ChicoMisiones", id: 4 },
				{ playerName: "HawkDiego", id: 5 },
				{ playerName: "Jorge Barón", id: 6 },
				{ playerName: "Neosphere", id: 7 },
			],
			playersMid: [
				{ playerName: "TheGameofLove69", id: 8 },
				{ playerName: "XxGeremiasxX", id: 9 },
			],
			playersAdc: [
				{ playerName: "SniperWolf919", id: 10 },
				{ playerName: "Sasquatchs", id: 11 },
			],
			playersSupp: [
				{ playerName: "Puntazo69420", id: 12 },
				{ playerName: "StallmanLover", id: 13 },
				{ playerName: "thezoneomega", id: 14 },
				{ playerName: "LeaderBak", id: 15 },
				{ playerName: "Heinf13ld", id: 16 },
			],
		};
	},
	components: {
		PositionListComponent,
	},
};
</script>

<style scoped>
.positions-lists {
	padding: 20px 0;
	width: 100%;
	height: 32%;
	display: flex;
	justify-content: center;
	gap: 2%;
}
</style>
