<footer>
	<div>

	</div>
	<div>

	</div>
	<div class="hide">
		<!-- <h4>Services</h4>
		<a href="/contact">Event Packages</a>
		<a href="/contact">Equipment Rental</a>
		<a href="/contact">DJ Hire</a> -->
	</div>
	<div class="full-width">
		<a href = "mailto: mufaez@gmail.com">Website created by Mufaez © 2022</a>
	</div>
</footer>

<style lang="scss">
	footer {
		width: 100vw;
		display: flex;
		flex-wrap: wrap;
		justify-content: space-evenly;
		background-color: #5cbcd6;
		color: white ;
		div {
			display: flex;
			flex-direction: column;
			align-items: center;
			min-width: 200px;
			margin: 20px 0;
			a {
				color: white;
				text-decoration: none;
			}
			&.full-width {
				min-width: 100vw;
			}
		}
		@media screen and (max-width: 600px) {
			.hide {
				display: none;
			}
		}
	}
</style>
