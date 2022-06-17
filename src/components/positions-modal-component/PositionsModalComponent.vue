<template>
	<div class="positions-container">
		<div class="positions-modal">
			<div class="position">
				<img
					class="position__img"
					src="../../assets/Position_Gold-Top.png"
					alt="top's position"
				/>
				<p class="position__name">TOP</p>
			</div>

			<div class="position">
				<img
					class="position__img"
					src="../../assets/Position_Gold-Jungle.png"
					alt="top's position"
				/>
				<p class="position__name">JUNGLA</p>
			</div>

			<div class="position">
				<img
					class="position__img"
					src="../../assets/Position_Gold-Mid.png"
					alt="top's position"
				/>
				<p class="position__name">CENTRAL</p>
			</div>

			<div class="position">
				<img
					class="position__img"
					src="../../assets/Position_Gold-Bot.png"
					alt="top's position"
				/>
				<p class="position__name">INFERIOR</p>
			</div>

			<div class="position">
				<img
					class="position__img"
					src="../../assets/Position_Gold-Support.png"
					alt="top's position"
				/>
				<p class="position__name">SUPORTE</p>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "PositionsModalComponent",
};
</script>

<style scoped>
.positions-container {
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
	background: rgba(0, 0, 0, 0.2);
}

.positions-modal {
	border: 3px solid goldenrod;
	box-shadow: 0px 0px 5px black;
	background: #0d2c54;
	padding: 35px 30px;
	display: flex;
	justify-content: center;
	gap: 30px;
	position: absolute;
	top: 30%;
	left: 50%;
	transform: translateX(-50%);
}

.position {
	display: flex;
	flex-direction: column;
	align-items: center;
	gap: 10px;
	color: #deb841;
	font-weight: bold;
	cursor: pointer;
}
</style>
