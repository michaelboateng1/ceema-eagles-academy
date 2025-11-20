<script>
	import image from '$lib/assets/images/children-1144109_1280.jpg';
</script>

<section
	class="container mx-auto mt-50 mb-20 flex h-auto items-start justify-start sm:h-[300px] md:px-5 lg:px-30"
>
	<div class=" hidden h-full w-full overflow-hidden bg-white sm:block">
		<img src={image} alt="" class="h-full w-full object-cover" />
	</div>
	<div class="h-full bg-[#e07b1c] p-5 text-white sm:p-10">
		<p class="quote relative pt-16 italic sm:pl-10">
			Ceema Eagles Academy transformed my approach to learning. The robotics program sparked my interest in technology, and the supportive teachers helped me build confidence in my coding skills. I've made incredible progress in just a few months!
		</p>

		<div class="mt-10 px-10 pb-10 sm:pb-0">
			<h3 class="text-md font-bold">James Bonsu</h3>
			<p class="text-sm">JHS-3 Student</p>
		</div>
	</div>
</section>

<style>
	.quote::before {
		content: '\275D';
		font-size: 3rem;
		float: left;
		clear: both;
		position: absolute;
		top: 20px;
		left: 0px;
	}
	.quote::after {
		content: '\275E';
		font-size: 3rem;
		float: right;
		position: absolute;
		right: 20px;
	}
</style>
