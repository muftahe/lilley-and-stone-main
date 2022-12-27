<script lang="ts">
	export let number: number;
	export let icon: string = '';
	export let title: string;
	export let body: string;
</script>

<main>
	<div>
		{#if icon}
			<img src={icon} alt="Saving Lilly & Stone" />
		{:else}
			<h2>0{number}</h2>
		{/if}
	</div>

	<h3>{title}</h3>
	<p>{body}</p>
</main>

<style lang="scss">
	@import url('https://fonts.googleapis.com/css2?family=Prompt:wght@500&display=swap');



	main {
		display: flex;
		align-items: center;
		flex-direction: column;
		margin-top: 50px;
		background-color: white;
		border: 2px solid black;
		border-radius: 80px;
		margin-left: 3%;
		margin-right: 3%;
		@media only screen and (min-width: 768px) { 
			margin-right: 10%;
			margin-left: 10%;
		}

	


	

		
		
		div {
			margin-top: 50px;
		
			background-color: #fff;
			border-radius: 100%;
			display: inline-block;
			width: 2.5em;
			height: 2.5em;
			font-size: 2em;
			display: flex;
			justify-content: center;
			align-items: center;

			img {
				height: 70%;
				width: 70%;
			}
		}
		// h2 {
		// 	display: flex;
		// 	justify-content: center;
		// 	align-items: center;
		// }

		h3 {
			margin-top: 15px;
			font-family: 'Prompt', sans-serif;
			font-weight: 800;
			font-size: 26px;
			text-align: center;
		}

		p {
			font-size: 15px;
			text-align: center;
			max-width: 80%;
			line-height: 1.6;
			margin-top: 10px;
			margin-bottom: 50px;
		}
		@media only screen and (min-width: 768px) {
			p {
				font-size: 18px;
			}
	}
}
</style>
