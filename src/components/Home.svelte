<script>
	import Header from './Header.svelte';
	import PageFrame from './PageFrame.svelte';
 	const base = (process['env']['isProd']) ? '' : ''
</script>

<main 	class="container-fluid h-100 d-flex flex-column" 
		style="background-image: url('{base+'/'}Hero.png'); background-size: cover; background-position: center center; background-repeat: no-repeat; overflow: hidden;">      
	<Header />
	<PageFrame>
		<div class="row" style="flex: 1 1 auto; background-color: rgba(116,255,116, 0.0);">
			<div class="col-md-6 align-self-center text-start" style="background-color: rgba(216,191,216, 0.0);">
				<img alt="Signature as SVG" src="{base}/logo.svg" style="width: 70%">
			</div>
			<div class="col-md-6"></div>
		</div>      
		<div class="row" style="flex: 1 1 auto; background-color: rgba(116,100,216, 0)">
			<div class="col-md-12 align-self-center text-end" style="background-color: rgba(116,200,216, 0.0); color: #DEB79A; font-size: 2.5em;">
				<p>Best New Music award winner 2013, Brass Band World</p>
				<p><i>“...a composer in possession of a mind bursting with ideas... Goldberg 2012 also showed a rare depth of musicality. “</i></p>
				<p>Philip Harper</p>
			</div>
		</div>                        
	</PageFrame>
</main>
