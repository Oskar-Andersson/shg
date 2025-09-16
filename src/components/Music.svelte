<script>
	import Header from './Header.svelte';
	import PageFrame from './PageFrame.svelte';
	import Footer from './Footer.svelte';
 	const base = (process['env']['isProd']) ? '' : ''	
</script>

<main class="container-fluid h-100 d-flex flex-column" style="background-image: url('{base+'/'}AdobeStock_246360083.jpeg'); background-size: cover; background-position: center center; background-repeat: no-repeat; overflow: hidden;">      
	<Header title={'Music'} />
	<PageFrame>

        <div class="row">
            
			<div class="col-md-6">                				
				<div class="row align-self-center" style="background-color: rgb(200,10,100, 0.0); flex: 1 1 auto;">
                    <div class="col-md-5 videocard videocard">
                        <div class="video-container">
                            <iframe class="video" src="https://www.youtube.com/embed/IWmGbdepTWs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                        </div>                                                
						<p>With Arctic Philharmonic<br>
						Force of Nature, by Svein Henrik Giske</p>
                    </div>
					<div class="col-md-1"></div>
                    <div class="col-md-5 videocard">                        
                        <div class="video-container">
                            <iframe class="video" src="https://www.youtube.com/embed/gd-IQOw7mk4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                        </div>                        
						<p>With Bergen Treblåsensemble (B3)<br>
						Marsj etter Erling Kjøk, by Svein Henrik Giske</p>
                    </div>
					<div class="col-md-1"></div>
                </div>
				<div class="row align-self-center" style="background-color: rgb(200,10,100, 0.0); flex: 1 1 auto;">
                    <div class="col-md-5 videocard">
                        <div class="video-container">
                            <iframe class="video" src="https://www.youtube.com/embed/lxY71FHakIk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                        </div>                                                
						<p>With Bergen Treblåsensemble (B3)<br>
						Mitt hjerte alltid vanker, by Svein Henrik Giske</p>
                    </div>
					<div class="col-md-1"></div>
                    <div class="col-md-5 videocard">                        
                        <div class="video-container">
                            <iframe class="video" src="https://www.youtube.com/embed/cO2DGQDz4Sg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                        </div>                        
						<p>With Bergen Treblåsensemble (B3)<br>
						Another Ground, by Svein Henrik Giske</p>
                    </div>
					<div class="col-md-1"></div>
                </div>
				<div class="row align-self-center" style="background-color: rgb(200,10,100, 0.0); flex: 1 1 auto;">
                    <div class="col-md-5 videocard">
                        <div class="video-container">
                            <iframe class="video" src="https://www.youtube.com/embed/N2nmftt5x7o" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                        </div>                                                
						<p>With Dragefjellets Musikkorps<br>
						Goldberg 2012, by Svein Henrik Giske</p>
                    </div>
					<div class="col-md-1"></div>
                    <div class="col-md-5 videocard">                        
                        <div class="video-container">
                            <iframe class="video" src="https://www.youtube.com/embed/-fAOqPfzjFY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                        </div>                        
						<p>With Sjøforsvarets Musikkorps (Royal Norwegain Naval Forces)<br>
						Jubileumsmarsj, by Svein Henrik Giske</p>
                    </div>
					<div class="col-md-1"></div>
                </div>
            </div>

            <div class="col-md-6 " style="TEXT-ALIGN: JUSTIFY">
                <div class="container" style=" background-color: rgba(0,0,0,0.4); padding: 20px; border-radius: 2px;">					
					<h3>Svein Henrik Giskes list of works since 1995:</h3>
					<p><span style="margin-right: 20px;">1995</span> 	A footpath from a human perspective (brass band)</p>
					<p><span style="margin-right: 20px;">1997</span>	Concertino for brass band</p>
					<p><span style="margin-right: 20px;">1998</span>	Introduction for brass band	</p>
					<p><span style="margin-right: 20px;">1999</span> 	Rukan Krukan (wind band)</p>
					<p><span style="margin-right: 20px;">2000</span> 	Following the waves (wind band)</p>
					<p><span style="margin-right: 20px;">2002</span>	Fragmotion (wind band)</p>
					<p><span style="margin-right: 20px;">2003</span> 	Nu rinner solen opp (brass band)</p>
					<p><span style="margin-right: 20px;">2005</span>	Til Siri (organ and saxophone)</p>
					<p><span style="margin-right: 20px;">2006</span> 	Herregud, ditt dyre navn og ære -fantasi- (big band)</p>
					<p><span style="margin-right: 20px;">2007</span> 	Forsvinn! -fantasi- (brass band)</p>
					<p><span style="margin-right: 20px;">2007</span>	Gjendines dance... and lullaby, -fantasi- (brass band)</p>
					<p><span style="margin-right: 20px;">2008</span>	Dance augmented (brass band)</p>
					<p><span style="margin-right: 20px;">2008</span>  	Three gentle giants (brass band)</p>
					<p><span style="margin-right: 20px;">2009</span>	Solefald (wind band and trombone soloist)</p>
					<p><span style="margin-right: 20px;">2009</span>	På tur med Nystemt'n, -fantasi- (wind band)</p>
					<p><span style="margin-right: 20px;">2010</span> 	New lines (flute, bassoon, horn and piano)</p>
					<p><span style="margin-right: 20px;">2010</span>	Flyt (brass band and trompet soloist)</p>
					<p><span style="margin-right: 20px;">2010</span>  	H.M. Dronning Sonjas honnørmarsj (brass band and wind band)</p>
					<p><span style="margin-right: 20px;">2010</span> 	Mitt hjerte alltid vanker, -fantasi- (woodwind ensemble)</p>
					<p><span style="margin-right: 20px;">2011</span> 	Goldberg 2012 (brass band)</p>
					<p><span style="margin-right: 20px;">2011</span>	The Maple Hawk o-phone (soprano saxophone and vibraphone)</p>
					<p><span style="margin-right: 20px;">2012</span> 	Some winters day (sinfonietta)</p>
					<p><span style="margin-right: 20px;">2012</span> 	Oppstigning! fanfare (wind band)</p>
					<p><span style="margin-right: 20px;">2012</span>	Liquid glass painting	(wind band)</p>
					<p><span style="margin-right: 20px;">2013</span> 	Roses on the tomb of Dido, Queen of Carthage (string quintet)</p>
					<p><span style="margin-right: 20px;">2013</span> 	Dark. Light. In between (wind band)</p>
					<p><span style="margin-right: 20px;">2013</span>	Another ground part 1 (woodwind ensemble and saxophone quartet) With support from Komponistenes Vederlagsfond.</p>
					<p><span style="margin-right: 20px;">2013</span> 	Jubileumsmarsj (wind band)</p>
					<p><span style="margin-right: 20px;">2014</span>	Pater Noster (mixed choir)</p>
					<p><span style="margin-right: 20px;">2014</span> 	Signs of Spring (bassoon, trumpet, percussion, harp, piano, violin and double bass)</p>
					<p><span style="margin-right: 20px;">2014</span>  	Solos (wind band with soloists: flute, soprano saxophone, cor anglais, bassoon and  vibraphone)</p>
					<p><span style="margin-right: 20px;">2014</span>	Another ground -complete version-(woodwind ensemble and saxophone quartet) With support from Komponistenes Vederlagsfond.</p>
					<p><span style="margin-right: 20px;">2015</span> 	Sons of Zeus for 2 trombones og brass band. Dedicated to soloists Marius Hesby, Grethe Tonheim and conductor Ingar Bergby. With support from Det Norske Komponistfond.</p>
					<p><span style="margin-right: 20px;">2016</span>	Force of Nature. For trombone soloist Ian Bousfield and strings from Arctic Philharmonic for the 2016 Arctic Trombone Festival. With support from Det Norske Komponistfond.</p>
					<p><span style="margin-right: 20px;">2018</span>	Made in Bergen (wind band)</p>
					<p><span style="margin-right: 20px;">2018</span>	Vox Clara (wind band med obosolist) With support from Morten E. Pedersens Minnefond</p>
					<p><span style="margin-right: 20px;">2021</span> 	New piece for brass band </p>
					<div class="d-flex" style="margin-top: 35px;">
					  <div class="flex-shrink-0">
					    <a href="https://notebutikken.no"><img alt="notebutikken.no logo" src="{base}/243568640_567675314284568_1604512146275012525_n.png"></a>
					  </div>
					  <div class="flex-grow-1 ms-3">
					   <p>Visit noteservice to purchase music, or contact the composer</p>
					  </div>
					</div>					
        <span style="margin-right: 20px;">    </span>    </div>
            </div>
        </div>
		<Footer />
	</PageFrame>
</main>

<style>
.video-container {
  position: relative;
  width: 100%;
  padding-bottom: 56.25%;
  margin-bottom: 10px;
}
.video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border: 0;
}
.videocard {
	background-color: rgba(0,0,0,0.3); 
	padding: 10px; 	
	padding-bottom: 0;	
	margin-bottom: 10px;
	border-radius: 2px;
}
p {
	color: #DFB898;
}
h3 {
	color: #DFB898;
}
</style>