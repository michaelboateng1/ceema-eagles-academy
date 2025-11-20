<script>
	import image from '$lib/assets/images/children-4768404_1280.jpg';
</script>

<section class="container mx-auto mt-60 mb-20 flex items-center justify-center gap-8 px-5 lg:px-30">
	<div>
		<h2 class="mb-2 text-xl font-bold uppercase sm:text-2xl">
			All students and stuff will feel safe & respected at sva
		</h2>
		<p class="mb-5 text-[#333]">
			The school environment (social, physical, emotional and behavioral) will be safe, welcoming,
			and conducive to learing.
		</p>
		<ul class="space-y-3 px-10 text-sm text-[#333]">
			<li>
				Our dedicated counseling team provides personalized support to ensure every student's emotional and academic needs are met.
			</li>
			<li>
				We maintain a zero-tolerance policy against bullying, with comprehensive anti-bullying programs and peer support systems.
			</li>
			<li>
				Regular mental health workshops and stress management sessions help students develop resilience and healthy coping mechanisms.
			</li>
		</ul>
	</div>

	<div class="hidden h-auto w-full overflow-hidden rounded-lg sm:block">
		<img src={image} alt="" class="h-full w-full object-cover" />
	</div>
</section>

<style>
	ul {
		list-style-image: url('../../lib/assets/checkmark-svgrepo-com.svg');
	}
</style>
