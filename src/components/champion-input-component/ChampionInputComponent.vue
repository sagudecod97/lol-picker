<template>
	<div class="champion-input">
		<input
			class="champion-input__champion"
			type="text"
			placeholder="Ingresa tu nombre de Invocador"
		/>

		<button class="champion-input__rol">Línea</button>

		<div class="champion-input__container">
			<svg
				xmlns="http://www.w3.org/2000/svg"
				class="champion-input__icon"
				fill="none"
				viewBox="0 0 24 24"
				stroke="currentColor"
				stroke-width="2"
			>
				<path
					stroke-linecap="round"
					stroke-linejoin="round"
					d="M14 5l7 7m0 0l-7 7m7-7H3"
				/>
			</svg>
		</div>
	</div>
</template>

<script>
export default {
	name: "ChampionInputComponent",
};
</script>

<style scoped>
.champion-input {
	display: flex;
	justify-content: center;
	gap: 20px;
	padding: 30px 0 10px 0;
}

.champion-input__champion {
	height: 45px;
	min-width: 300px;
	padding: 5px;
	font-size: 18px;
	border: 1px solid goldenrod;
	background: #0d2c54;
	color: goldenrod;
	box-shadow: 0px 0px 5px black;
}

.champion-input__rol {
	border: 1px solid goldenrod;
	color: #deb841;
	font-size: 18px;
	background: #0d2c54;
	padding: 0 5px;
	cursor: pointer;
	box-shadow: 0px 0px 5px black;
}

.champion-input__container {
	width: 45px;
	height: 45px;
	border: 1px solid goldenrod;
	background: #0d2c54;
	border-radius: 50%;
	padding: 5px;
	box-shadow: 0px 0px 5px black;
}

.champion-input__icon {
	border-radius: 100%;
	padding: 2px;
	color: #deb841;
	cursor: pointer;
}
</style>
