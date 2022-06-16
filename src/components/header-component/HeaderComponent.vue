<template>
	<header class="header">
		<div class="header__container">
			<img
				class="header__img"
				src="../../assets/League-of-legends-logo.png"
				alt="League of Legend's logo"
			/>
		</div>
	</header>
</template>

<script>
export default {
	name: "HeaderComponent",
};
</script>

<style scoped>
.header {
	width: 100%;
	height: 18%;
}

.header__container {
	width: 20%;
	height: 100%;
	margin: 0 auto;
	display: flex;
	justify-content: center;
}

.header__img {
	width: auto;
	height: 100%;
	margin: auto;
}
</style>
