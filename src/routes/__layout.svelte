<svelte:head>
	<link rel="stylesheet" href="/reset.css">
</svelte:head>

<script>
  import Header from '../components/header.svelte';
</script>

<Header />
<main>
  <slot></slot>
</main>
<footer>footer</footer>