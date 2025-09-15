<script>
	import Header from './Header.svelte';
	import PageFrame from './PageFrame.svelte';
	import Footer from './Footer.svelte';
 	const base = (process['env']['isProd']) ? '/shg' : ''	
	const images = [
		{
			active: true,		
			descr: 'Photo by Hege Haukefær',
			photo: '/carousel/DSC_0388.png',
		},
	/* 	{
			descr: 'Photo by Hege Haukefær',
			photo: '/carousel/DSC_0398.png',
		},
		{
			header: 'First slide label',
			descr: 'Private photo',
			photo: '/carousel/243027282_677109306588614_5187655386732845063_n.jpg',	
		}, */
		{
			descr: 'Photo by Sissel Grønlund',
			photo: '/carousel/243127189_161596956144376_1105875297059653370_n.jpg',	
		},
		{
			photo: '/carousel/243127925_4337010529680261_2252309596895278791_n.jpg',	
		},
		{
			photo: '/carousel/243161108_1186710121839618_5789436727830739854_n.jpg',
		},
		{
			photo: '/carousel/243400726_591321095555552_3333375961966169838_n.jpg',
		},
		// {
		// 	photo: '/carousel/243448945_394068972316024_6023593568879375735_n.jpg',
		// },
		{
			photo: '/carousel/close up.png',
		},
		// {
		// 	photo: '/carousel/DSC_0390.png',
		// },
		{
			photo: '/carousel/DSC_0416.png',
		},
		{
			photo: '/carousel/DSC_0424.png',
		},
		// {
		// 	photo: '/carousel/DSC_0451.png',
		// },
		{
			photo: '/carousel/DSC_0465 copy.png',
		},
		{
			photo: '/carousel/fingers.trumpet.png',
		},
		// {
		// 	photo: '/carousel/ian.bousfield.png',
		// },
		{
			photo: '/carousel/musikkforeleggerprisen.png',
		},
		{
			photo: '/carousel/portrett1.png',
		},
		{
			photo: '/carousel/Skjermbilde 2015-11-05 kl. 11.06.45.png',
		},
		{
			photo: '/dragen-ha1.jpg',
			header: 'Svein H. Giske conducting a concert at Grieghallen, Bergen',
			descr: 'Dragefjellets musikkorps. Photo Ingvild Festervoll Melien',
		}		           
	]
	
	const buttons = [...images]
	buttons.shift()
	
</script>

<main class="container-fluid h-100 d-flex flex-column" style="background-image: url('{base+'/'}AdobeStock_173509560.jpeg'); background-size: cover; background-position: center center; background-repeat: no-repeat; overflow: hidden;">      
	<Header title={'Gallery'} />
	<PageFrame>

		<div id="carouselExampleCaptions" class="carousel slide" data-bs-ride="carousel">
		<div class="carousel-indicators">
			<ol class="carousel-indicators">
				<li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
				<li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
				<li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
			</ol>

			<button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
			{#each buttons as _, i}
    			<button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="{i+1}" aria-label="Slide {i+2}"></button>
			{/each}
			
		</div>
		<div class="carousel-inner">
			{#each images as _, i}
			<div class="carousel-item {_.active ? 'active' : ''}">
			<img src="{base}{_.photo}" alt="..." class="d-block">
			<div class="carousel-caption d-none d-md-block"> 				
				{#if _.header}<h5>{_.header}</h5>{/if}
				{#if _.descr}<p>{_.descr}</p>{/if}								
			</div>
			</div>
			{/each}

		</div>
		<button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="prev">
			<span class="carousel-control-prev-icon" aria-hidden="true"></span>
			<span class="visually-hidden">Previous</span>
		</button>
		<button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="next">
			<span class="carousel-control-next-icon" aria-hidden="true"></span>
			<span class="visually-hidden">Next</span>
		</button>
		</div>

		<Footer />
	</PageFrame>
</main>

<style>
img {
	margin: auto; 
	width: auto;  
	max-height:800px;
	min-height:800px;
}

</style>