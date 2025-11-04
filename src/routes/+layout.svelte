<script>
	import '../app.css';
	import favicon from '$lib/assets/images/get.jpeg';

	import Footer from './components/Footer.svelte';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children?.()}
<Footer />

<!-- #e07b1c -->