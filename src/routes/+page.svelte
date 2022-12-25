

<link rel = "stylesheet" href = "/src/routes/page.css">

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
	import hero5 from '$lib/assets/tennis/1.png'
	import circleStop from '$lib/assets/logos/circle-stop-regular.svg';
	import consult from '$lib/assets/logos/person-chalkboard-solid.svg';
	import { add_resize_listener } from 'svelte/internal';
</script>

<main>
	<Hero
		image={{ src: hero5, alt: 'Saving Lilley and Stone' }}
		header="Saving Lilley and Stone"
	/>
<br><br>
	<div class = "textimage">

		<h1 style="margin-bottom: 1rem">WE DEEPLY CARE ABOUT OUR TOWN</h1><br>
		<p> Our town is rich in history, buildings, green spaces, educational and cultural facilities </p>
		<br>
		<p>We want to maintain the day-to-day quality of life for our residents and build a future legacy for our children and the next generation</p>
		<br>
		<p>The Lilley and Stone site is central to this and thus we feel moved to act</p>

	</div>
<br><br><br><br><br><br>
	<h1>OUR OBJECTIVES</h1>
	<List title = "_"
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
	<div class="petition">
		<a href="/">Sign our petition</a>
	</div>
<br><br><br>
</main>

<style lang="scss">

	@import url('https://fonts.googleapis.com/css2?family=Prompt:wght@500&display=swap');

	.s-GopaBODuPFzn {
		font-family: 'Prompt', sans-serif;

	}

	.s-y_bCXRrkrYfP {
    background-color: #ebeefb;
}
	a {
		margin-left: 50%;
		margin-right: 50%;
	}
	h1 {
		font-family: 'Prompt', sans-serif;
		font-size: 40px;
		text-align: center;
	}
	ul {
		list-style-position: inside;
		font-family: 'Prompt', sans-serif;
	}
	.petition {
		margin-top: 50px;
		width: 100vw;
		font-family: 'Prompt', sans-serif;
		display: flex;
		/**height: 10vh;*/
		justify-content: center;
		align-items: center;
		/**margin: 3em 0;*/
		a {
			text-decoration: none;
			color: black;
			font-family: 'Prompt', sans-serif;
			background-color: white;
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
			width: 100px;
			height: 100px;
		}
		50% {
			width: 150px;
			height: 150px;
		}
		100% {
			width: 100px;
			height: 100px;
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
