<template>
	<main class="main-component">
		<champion-input-component />
		<champions-component />
		<positions-lists-component />
	</main>
</template>

<script>
import ChampionInputComponent from "../champion-input-component/ChampionInputComponent.vue";
import ChampionsComponent from "../champions-component/ChampionsComponent.vue";
import PositionsListsComponent from "../positions-lists-component/PositionsListsComponent.vue";

export default {
	name: "MainComponent",
	components: {
		ChampionInputComponent,
		ChampionsComponent,
		PositionsListsComponent,
	},
};
</script>

<style scoped>
.main-component {
	width: 100%;
	height: 82%;
}
</style>
