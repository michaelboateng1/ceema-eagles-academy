<script>
    import { onMount } from 'svelte';
    import NavBar from "./NavBar.svelte";

    const {page} = $props();

    let scrolled = $state(false);

	onMount(() => {

		scrolled = window.scrollY > 838;

		const handleScroll = () => {
			scrolled = window.scrollY > 838;
		};

		window.addEventListener('scroll', handleScroll);
        
		return () => window.removeEventListener('scroll', handleScroll);
	});
</script>

<header class="fixed top-0 z-10 w-full transition-all duration-300 {scrolled || page !== "home" ? 'bg-white text-[#333] shadow-md' : 'header-bg text-white'}">
    <NavBar />
</header>

<style>
    .header-bg {
        background-color: hsla(0, 0%, 39%, 0.5);
    }
</style>
