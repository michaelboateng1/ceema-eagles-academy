<script>
	import '../app.css';
	import favicon from '$lib/assets/images/schoolLogo.jpg';

	import AOS from 'aos';
	import 'aos/dist/aos.css';

	import Footer from './components/Footer.svelte';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children?.()}
<Footer />

<!-- #e07b1c -->
