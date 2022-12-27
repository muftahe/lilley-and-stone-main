<script lang="ts">
	export let image: {
		src: string;
		alt: string;
	};
	export let header: string = '';
	export let sub: string = '';
</script>

<section>
	<img src={image.src} alt={image.alt} />
	<h1>WE NEED YOUR HELP</h1>
	{#if sub}
		<h3>{sub}</h3>
	{/if}
</section>

<style lang="scss">



	section {
		position: relative;
		height:60vh;
		background-color: white;
		img {
			display: block;
			position: absolute;
			width: 100%;
			height: 150%;
			object-fit: cover;
			animation: fadeout 1s ease forwards;
			background-color: white;
		}
		h1 {
			/**font-family: 'Island Moments', cursive;*/
			position: absolute;
			color: black;
			display: none;
			background-color: white;
			top: 50%;
			left: 50%;
			transform: translate(-50%, 0);
			font-size: 4em;
			text-align: center;
			animation: slideup 1s ease forwards;
		}
	}

	@keyframes slideup {
		0% {
			opacity: 0;
		}
		100% {
			opacity: 1;
			transform: translate(-50%, -50%);
		}
	}

	/**@keyframes fadeout {
		0% {
			opacity: 1;
		}
		100% {
			opacity: 0.7;
		}
	}*/
</style>
