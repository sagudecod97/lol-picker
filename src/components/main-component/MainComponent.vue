<template>
	<main class="main-component">
		<champion-input-component />
	</main>
</template>

<script>
import ChampionInputComponent from "../champion-input-component/ChampionInputComponent.vue";

export default {
	name: "MainComponent",
	components: {
		ChampionInputComponent,
	},
};
</script>

<style scoped>
.main-component {
	width: 100%;
	height: 82%;
}
</style>
