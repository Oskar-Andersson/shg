<script>
  import { onMount } from 'svelte';

  import Home from './components/Home.svelte';
  import Bio from './components/Bio.svelte';
  import Music from './components/Music.svelte';
  import Gallery from './components/Gallery.svelte';
  import Contact from './components/Contact.svelte';
  import NotFound from './components/NotFound.svelte';

  let current = Home;

  function pick(pathname) {
    const p = (pathname.replace(/\/+$/,'') || '/').toLowerCase();
    if (p === '/')        return Home;
    if (p === '/bio')     return Bio;
    if (p === '/music')   return Music;
    if (p === '/gallery') return Gallery;
    if (p === '/contact') return Contact;
    return NotFound;
  }

  function renderFor(pathname) {
    current = pick(pathname);
  }

  function navigate(to) {
    if (location.pathname !== to) history.pushState({}, '', to);
    renderFor(to);
  }

  // Event delegation: intercept clicks on <a href="/...">
  function onClick(e) {
    // left click, no modifiers, anchor with same-origin absolute path
    if (e.defaultPrevented || e.button !== 0 || e.metaKey || e.ctrlKey || e.shiftKey || e.altKey) return;
    let a = e.target;
    while (a && a.nodeName !== 'A') a = a.parentNode;
    if (!a || a.target || a.hasAttribute('download')) return;

    const href = a.getAttribute('href');
    if (!href || !href.startsWith('/')) return; // external/relative links ignored

    e.preventDefault();
    navigate(href);
  }

  onMount(() => {
    // initial render for deep link
    renderFor(location.pathname);
    // client-side nav + back/forward
    window.addEventListener('click', onClick);
    window.addEventListener('popstate', () => renderFor(location.pathname));
  });
</script>

<svelte:component this={current} />
