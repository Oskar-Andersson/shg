<script>
	import Header from './Header.svelte';
	import PageFrame from './PageFrame.svelte';
    import Footer from './Footer.svelte';
  	const base = (process['env']['isProd']) ? '/shg' : ''
</script>

<main class="container-fluid d-flex flex-column h-100" style="background-image: url('{base+'/'}AdobeStock_128726374.jpeg'); background-size: cover; overflow: hidden;">      
	<Header title={'Biography'} />
	<PageFrame>        
        <div class="row">
            <div class="col-md-4 d-flex flex-column ">
                <div class="row d-flex flex-colum align-self-center" style="background-color: rgb(200,10,100, 0.0);">
                    <div class="col-md-auto">
                        <img alt="Portrait of Sven H. Giske" src="{base}/portrett1.png" style="width: 100%;"> 
                    </div>
                </div>
                <div class="row d-flex flex-colum align-self-center" style="width: 100%; margin: 10px; background-color: rgb(200,10,100, 0.0); flex: 1 1 auto;">
                    <div class="col-md-12" style="padding: 0;">                        
                        <div class="video-container">
                            <iframe class="video" src="https://www.youtube.com/embed/N2nmftt5x7o" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                        </div>                        
                    </div>
                </div>
            </div>
            <div class="col-md-8">
                <div class="container">
                <p>
                Svein H. Giske was born in Ålesund on the northwestern coast of Norway in 1973.                 
                From 1993 he's been located in Bergen, where he studied trumpet at the Grieg Academy.                
                In 1996 he landed a position as a trumpeter in The Norwegian Naval Forces' Band in Bergen where he still works. He is a frequent soloist with the band both in live performances and on recordings.                 
                Giske is versatile both as a trumpet player and as a composer/arranger. 
                From 1997 to date he's been a permanent member of the Bergen Big Band. He has also on many occasions played with contemporary ensemble Bit 20 and the Bergen Philharmonic Orchestra.                  
                Giske has also worked several years at Den Nationale Scene, the theatre in Bergen, and on musicals and shows as a freelancer. 
                </p>
                <p>
                Giske studied composition with Morten E. Pedersen at the Grieg Academy.
                He has written and arranged a lot of music, mainly for winds and percussion, but also for choir, big band and various chamber music constellations. 
                His music is often rhythmically driven, with influences from jazz and pop as well as classical and contemporary music. Although pulse and rhythm is important to Giske, he also has a strong lyrical and expressive vein running through his music.
                He has written for contemporary ensemble Bit 20, and has had commissions from 
                The Norwegian Band Federation with trumpet virtuoso Ole Edvard Antonsen, 
                The Arctic Philharmonic with trombone virtuoso Ian Bousfield, 
                The Norwegian Naval Forces' Band, Eikanger-Bjørsvik Musikklag, Stavanger Brass Band, Bergen Woodwind Ensemble (B3),The Bergen Big Band and several others. 
                
                He wrote Goldberg 2012 as a test piece for the Norwegian Band Federation. 
                After the premiere the same year, this piece won 2 awards; 
                Test Piece of the Year (4barsrest.com) and Best New Music (Brass Band World). 
                The wind band version was also nominated for the Norwegian Music Publishers' Award in 2020. 
                </p>

                <p>
                Giske has been working as a conductor from the early 2000s, mainly with brass bands and wind bands in the Bergen area. 
                He has long tenures with Dragefjellets Musikkorps and Askøy Brass Band and is musical director for both bands. 
                With Askøy, he's had 3 wins in the Siddis Brass Contest; in 2009, 2012 and 2019. 
                All programmes featured Giske's own arrangements. 
                </p>
                <!-- <div class="d-flex justify-content-center">
                    <figure class="figure w-100">
                    <img alt="Svein H. Giske conducting a concert at Grieghallen, Bergen"  class="w-100" src="{base}/dragen-ha1.jpg">
                    <figcaption class="figure-caption">Dragefjellets musikkorps. Photo Ingvild Festervoll Melien</figcaption>
                    </figure>                
                </div> -->
                <p>
                Giske has about 20 years experience of adjudicating bands, soloists and ensembles. He works both locally, regionally and in national contests.
                </p>
                </div>
            </div>
        </div>
        <Footer></Footer>        
	</PageFrame>
</main>

<style>
.video-container {
  position: relative;
  width: 100%;
  padding-bottom: 56.25%;
}
.video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border: 0;
}
.figure-caption {
    color: darkslategray;
}
p {
    font-family: 'Karla', sans-serif;
    font-weight:500;
    font-size: 14pt;
}
.container {
    background-color: rgba(255,255,255, 0.2);
    padding-left: 30px;
    padding-right: 30px;
    padding-top: 10px;
    padding-bottom: 5px;
    border-radius: 3px;

}
.hilite {
    color: rgb(142, 83, 54);    
}
</style>