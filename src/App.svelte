<script>	
	export const name = 'Svein H. Giske'
	import router from "page"
	import Home from './components/Home.svelte'
	import Bio from './components/Bio.svelte'
	import Music from './components/Music.svelte'
	import Gallery from './components/Gallery.svelte'
	import Contact from './components/Contact.svelte'
	import NotFound from './components/NotFound.svelte'	
	
	const base = (process['env']['isProd']) ? '/shg' : ''
	let page = null

	router('/', () => page = Home)
	router('/bio', () => page = Bio)
	router('/music', () => page = Music)
	router('/gallery', () => page = Gallery)
	router('/contact', () => page = Contact)
	router('/*', () => page = NotFound)

	if(process['env']['isProd']) router.base('/shg')
	router.start()
	
</script>
<svelte:head>
	    <base href="{base}" />
</svelte:head>
<svelte:component this={page} />
