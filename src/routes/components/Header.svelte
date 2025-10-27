<script>
    import { onMount } from 'svelte';
    import NavBar from "./NavBar.svelte";

    let scrolled = $state(false);

	onMount(() => {
		const handleScroll = () => {
			scrolled =  window.innerHeight - window.scrollY <= 15 || window.scrollY > 838;
		};
		window.addEventListener('scroll', handleScroll);
        window.addEventListener('DOMContentLoaded', handleScroll);
        
		return () => {
            window.removeEventListener('scroll', handleScroll);
            window.removeEventListener('DOMContentLoaded', handleScroll);

        };
	});
</script>

<header class="fixed top-0 z-10 w-full transition-all duration-300 {scrolled ? 'bg-white text-[#333] shadow-md' : 'header-bg text-white'}">
    <NavBar />
</header>

<style>
    .header-bg {
        background-color: hsla(0, 0%, 39%, 0.5);
    }
</style>
