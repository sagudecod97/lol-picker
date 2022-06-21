<template>
	<div class="champions">
		<div
			class="champion__champ --top"
			:style="{
				'background-image': `url(${require('../../assets/jg-rol-one.jpg')})`,
				'background-position': 'center',
				'background-repeat': 'no-repeat',
				'background-size': 'cover',
			}"
		>
			<div class="champion__tag">
				<p class="champion__name">Invocador</p>
			</div>
		</div>

		<div
			class="champion__champ --jg"
			:style="{
				'background-image': `url(${require('../../assets/jg-rol-one.jpg')})`,
				'background-position': 'center',
				'background-repeat': 'no-repeat',
				'background-size': 'cover',
			}"
		>
			<div class="champion__tag">
				<p class="champion__name">Invocador</p>
			</div>
		</div>

		<div
			class="champion__champ --mid"
			:style="{
				'background-image': `url(${require('../../assets/jg-rol-one.jpg')})`,
				'background-position': 'center',
				'background-repeat': 'no-repeat',
				'background-size': 'cover',
			}"
		>
			<div class="champion__tag">
				<p class="champion__name">Invocador</p>
			</div>
		</div>

		<div
			class="champion__champ --adc"
			:style="{
				'background-image': `url(${require('../../assets/jg-rol-one.jpg')})`,
				'background-position': 'center',
				'background-repeat': 'no-repeat',
				'background-size': 'cover',
			}"
		>
			<div class="champion__tag">
				<p class="champion__name">Invocador</p>
			</div>
		</div>

		<div
			class="champion__champ --supp"
			:style="{
				'background-image': `url(${require('../../assets/jg-rol-one.jpg')})`,
				'background-position': 'center',
				'background-repeat': 'no-repeat',
				'background-size': 'cover',
			}"
		>
			<div class="champion__tag">
				<p class="champion__name">Invocador</p>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "ChampionsComponent",
};
</script>

<style scoped>
.champions {
	width: 100%;
	height: 50%;
	display: flex;
	justify-content: center;
	gap: 2%;
	padding-top: 40px;
}

.champion__champ {
	border: 3px solid goldenrod;
	max-width: 250px;
	width: 100%;
	height: 100%;
	background: #0d2c54;
	box-shadow: 0px 0px 5px black;
	position: relative;
	background-repeat: no-repeat;
	background-size: cover;
}

.champion__img {
	height: 100%;
	width: auto;
}

.champion__tag {
	position: absolute;
	width: 110%;
	background: #0d2c54;
	border: 3px solid goldenrod;
	bottom: 4%;
	left: 50%;
	transform: translateX(-50%);
}

.champion__name {
	text-align: center;
	padding: 5px;
	font-size: 15px;
	color: #deb841;
	box-shadow: 0px 0px 5px black;
}
</style>
