<script>
	import Header from './Header.svelte';
	import PageFrame from './PageFrame.svelte';
	import Footer from './Footer.svelte';
  	const base = (process['env']['isProd']) ? '/shg' : ''
</script>

<main class="container-fluid h-100 d-flex flex-column" style="background-image: url('{base+'/'}AdobeStock_85241054.jpeg'); background-size: cover; background-position: center center; background-repeat: no-repeat; overflow: hidden;">      
	<Header title={'Contact'} />
	<PageFrame>
			<div class="row h-100 justify-content-center" style="flex: 1 1 auto;">
				<div class="col-12 col-xl-6 align-self-center justify-content-center card text-center">					
					<h2>Svein Henrik Giske</h2>
					<a href="mailto: sveinhgiske@gmail.com">sveinhgiske@gmail.com</a>
					<p>Phone +47 900 34 094</p>
				</div>
			</div>
		<Footer />
	</PageFrame>
</main>
<style>

	h2 {
		font-size: 2.5em; 
		font-weight:500;
		color: #2f3d4b
	}
	a {
		font-size: 1.5em; 
		color: #2f3d4b;	
		text-decoration: none;		
	}
	p {
		font-size: 1.5em; 
	}
	.card {
		font-family: 'PT Sans', sans-serif; 		
		color: #2f3d4b;
		background-color: rgba(255, 255, 255, 0.3);
		border-radius: 2px;
		height: 400px;
	}
</style>