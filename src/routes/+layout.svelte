<script>
	import '../app.css';
	import favicon from '$lib/assets/images/schoolLogo.jpg';

	import AOS from 'aos';
	import 'aos/dist/aos.css';

	import ChatBot from './components/ChatBot.svelte';
	import Footer from './components/Footer.svelte';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<ChatBot />
{@render children?.()}
<Footer />

<!-- #e07b1c -->
