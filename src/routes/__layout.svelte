<svelte:head>
	<link rel="stylesheet" href="/global.css">
</svelte:head>

<script>
  import '@fontsource/Outfit/400.css';
  import "@fontsource/Outfit/600.css";
  import "@fontsource/Outfit/700.css";
  import "@fontsource/material-icons-outlined";
  import Header from '$lib/header.svelte';
  import Footer from '$lib/footer.svelte';
</script>

<Header />
<main>
  <slot></slot>
</main>
<Footer />

<style>

  /* Typography */

  :global(html) {
    font-size: 10px;
  }

  :global(p) {
    font-size: 1.9rem;
    line-height: 1.2;
  }

  :global(.p-medium) {
    font-size: 2.4rem;
    line-height: 1.2;
  }

  :global(.p-large) {
    font-size: 2.8rem;
    line-height: 1.2;
  }

  :global(a) {
    transition: color .1s ease-out;
  }

  :global(a),
  :global(a:visited) {
    color: #337AB7;
  }

  :global(a:hover),
  :global(a:visited:hover) {
    color: #F7ACD4;
  }

  :global(.text-semibold) {
    font-weight: 600;
  }

  :global(.text-bold) {
    font-weight: 700;
  }

  :global(.text-blue) {
    color: #337AB7;
  }

  :global(.text-center) {
    text-align: center;
  }

  :global(.underline-pink) {
    position: relative;
  }

  :global(.underline-pink):after {
    position: absolute;
    content: '';
    width: 100%;
    height: 10px;
    background-color: #F7ACD4;
    left: 0;
    bottom: 17px;
    z-index: -1;
  }

  :global(.material-icons-outlined) {
  vertical-align: text-bottom;
}
</style>