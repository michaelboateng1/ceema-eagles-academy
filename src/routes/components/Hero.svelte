<script>
	import image1 from '$lib/assets/images/schoolLogo.jpg';
	import HeroCards from './HeroCards.svelte';
</script>

<section
	class="relative mb-20 flex h-screen w-full flex-col items-center justify-center px-5 sm:px-0"
>
	<div class="flex flex-col items-center justify-center">
		<div class=" mb-10 h-auto w-20 overflow-hidden rounded-lg sm:w-40">
			<img src={image1} alt="School Logo" class="object-fit h-full w-full" />
		</div>

		<div class="text-white">
			<div class="mb-5 flex flex-col items-center justify-center text-center">
				<h1 class=" poppins-extrabold mb-5 text-4xl font-bold sm:text-5xl">
					Join <span class="text-[#e07b1c]">Ceema Eagles</span> Today.
				</h1>
				<p class="text-center capitalize sm:w-[50ch]">
					We ensure better education for better world
				</p>
			</div>
			<div class="flex items-center justify-center gap-5 sm:gap-8">
				<a
					href="/conatct"
					class=" rounded-4xl border-2 border-[#e07b1c] bg-[#e07b1c] px-5 py-2 text-nowrap text-white transition-colors duration-300 hover:border-[#000] hover:bg-[#000] hover:text-white sm:px-10"
					>Conatct</a
				>
				<a
					href="admission"
					class=" rounded-4xl border-2 border-[#e07b1c] px-5 py-2 text-nowrap text-white transition-colors duration-300 hover:border-[#000] hover:bg-[#000] hover:text-white sm:px-10"
					>Join us</a
				>
			</div>
		</div>
	</div>

	<div class="absolute -bottom-20 container mx-auto flex items-center justify-center gap-8 px-30">
		<HeroCards />
		<HeroCards />
		<HeroCards />
	</div>
</section>

<style>
	section {
		background:
			linear-gradient(hsla(0, 0%, 20%, 0.5), hsla(0, 0%, 20%, 0.8)),
			url('../../lib/assets/images/get.jpeg');
		background-position: center;
		background-size: cover;
		background-repeat: no-repeat;
		background-attachment: fixed;
	}
</style>
