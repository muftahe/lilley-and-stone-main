

<script lang="ts">
	// components

	import Hero from '$lib/components/image/Hero.svelte';
	import CenterText from '$lib/components/text/CenterText.svelte';
	import TextImage from '$lib/components/image/TextImage.svelte';
	import LargeTextFromLeft from '$lib/components/text/LargeTextFromLeft.svelte';
	import List from '$lib/components/List/index.svelte';
	// images
	import pm_2 from '$lib/assets/meeting/pm_2.jpg';
	import building_2 from '$lib/assets/school/building_2.jpg';
	import hero5 from '$lib/assets/tennis/2.png'
	import circleStop from '$lib/assets/logos/circle-stop-regular.svg';
	import consult from '$lib/assets/logos/person-chalkboard-solid.svg';
	import { add_resize_listener } from 'svelte/internal';
</script>

<main>
	<!-- <p style ="font-family: 'Prompt', sans-serif; text-align: center; font-size: 2em; font-weight: 700; margin-bottom: -10px;">SAVING LILY AND STONE </p>-->
	
	<Hero
		image={{ src: hero5, alt: 'Saving Lilley and Stone' }}
		header="Saving Lilley and Stone"
	/>

<div class = "textimage">
<br>
		<h1 style="margin-bottom: 1rem; color: black;">WE DEEPLY CARE ABOUT OUR TOWN</h1><br>
		<p style ="color: black;"> Our town is rich in history, buildings, green spaces, educational and cultural facilities </p>
		<br>
		<p style ="color: black;">We want to maintain the day-to-day quality of life for our residents and build a future legacy for our children and the next generation. <br><br>The Lilley and Stone site is central to this and thus we feel moved to act</p>

<br><br><br>
</div>
<br><br><br><br><br><br>
	<h1>OUR OBJECTIVES</h1>
	<List title = "✓"
		cardDetails={[
			{
				title: 'Halt progress',
				body: 'Halt the rapid progress of this proposal by the trustees and their agents MLN.',
				icon: circleStop
			},
			{
				title: 'Consultation',
				body: 'We need a much longer consultation period to properly explore all other options.',
				icon: consult
			}
		]}
	/>

<br><br><br><br><br><br>

	<List title="WHAT WE OBJECT TO" />

	<!-- <div class="email-list">
		<h2 id="email-update">Enter your email for updates!</h2>
		<span>
			<label>Email</label>
			<input type="email" />
		</span>
	</div> -->

<br><br><br>

<br><br><br>
</main>

<div class="petition">
	<a href="/">Sign our petition</a>
</div>

<style lang="scss">



	@import url('https://fonts.googleapis.com/css2?family=Prompt:wght@500&display=swap');
	.textimage {
		margin-top: 60%;
		margin-bottom: -2%;
		
		margin-left: 5%;
		margin-right: 5%;
		@media only screen and (min-width: 768px) {
			p {
			margin-left: 5%;
			margin-right: 5%;
			}
		}

		text-align: center;
	}
	@media only screen and (min-width: 768px) {
  		.textimage {
    		margin-top: 20%;
			background-color: #fff;
		
		
  		}
	}

	.s-GopaBODuPFzn {
		font-family: 'Prompt', sans-serif;
	}
	main {
    background-color: #fff;
}
	a {
		margin-left: 50%;
		margin-right: 50%;
	}
	h1 {
		font-family: 'Prompt', sans-serif;
		font-size: 40px;
		text-align: center;
		margin: 20px;
	}
	p {
		margin-left: 20px;
		margin-right: 20px;
		justify-content: center;
	}
	ul {
		list-style-position: inside;
		font-family: 'Prompt', sans-serif;
	}
	.petition {
		width: 100vw;
		background-color: #fff;
		font-family: 'Prompt', sans-serif;
		display: flex;
		/**height: 10vh;*/
		justify-content: center;
		align-items: center;
		/**margin: 3em 0;*/
		a {
			margin-top: 1%;
			margin-bottom: 10%;
			text-decoration: none;
			color: black;
			font-family: 'Prompt', sans-serif;
			background-color: #68d7f6;
			
			border-radius: 100%;
			/**width: 50px;
			height: 50px;*/
			white-space: nowrap;
			display: flex;
			justify-content: center;
			align-items: center;
			transition: all 0.7s ease;
			animation: pulse 3s infinite ease;
			font-weight: 700;
			/**font-size: 1.5em;*/
			font-size: 2.5em;
			&:hover {
				width: 200px;
				height: 160px;
			}
		}
	}
	@keyframes pulse {
		0% {
			width: 150px;
			height: 150px;
		}
		50% {
			width: 200px;
			height: 200px;
		}
		100% {
			width: 150px;
			height: 150px;
		}
	}
	.email-list {
		width: 100%;
		height: 10vh;
		background-color: #ebeefb;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		h2 {
			margin-bottom: 1rem;
		}
	}
</style>