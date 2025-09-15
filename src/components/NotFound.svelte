<script>
	import Header from './Header.svelte';
	import PageFrame from './PageFrame.svelte';
</script>

<main class="container-fluid h-100 d-flex flex-column" style="background-image: url('Hero.png'); background-size: cover; background-position: center center; background-repeat: no-repeat; overflow: hidden;">      
	<Header />
	<PageFrame>
		<div class="row" style="flex: 1 1 auto; background-color: rgba(116,255,116, 0.0);">
			<div class="col-md-12 align-self-center text-center" style="background-color: rgba(216,191,216, 0.0);">		
				<h1 style="color: white"> 404 - Sorry page not found!</h1>
			</div>
		</div>
	</PageFrame>
</main>

<style>
	/* main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	} */
</style>