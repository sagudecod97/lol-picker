<template>
	<div class="app">
		<header-component />
		<main-component />
		<positions-modal-component />
	</div>
</template>

<script>
import HeaderComponent from "./components/header-component/HeaderComponent.vue";
import MainComponent from "./components/main-component/MainComponent.vue";
import PositionsModalComponent from "./components/positions-modal-component/PositionsModalComponent.vue";

export default {
	name: "App",
	components: {
		HeaderComponent,
		MainComponent,
		PositionsModalComponent,
	},
};
</script>

<style>
* {
	margin: 0;
	padding: 0;
	box-sizing: border-box;
}

.app {
	width: 100vw;
	height: 100vh;
	background-image: url("./assets/background.jpg");
	background-repeat: no-repeat;
	background-size: cover;
	background-position: center;
	position: relative;
}
</style>
