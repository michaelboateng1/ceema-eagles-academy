<script>
	import image from '$lib/assets/images/get.jpeg';
</script>

<section class="container mx-auto mt-40">
	<h1 class="mb-2 p-5 text-xl font-bold uppercase sm:p-4 sm:text-2xl">About us</h1>
	<div class="flex flex-col justify-between gap-8 px-5 sm:flex-row sm:px-0">
		<div class="space-y-5">
			<div class="space-y-4 border-l-4 border-[#e07b1c] bg-[#636363] p-4 text-[#ccc]">
				<div class="relative h-[45px] w-[45px] rounded-full bg-[#808080] text-4xl">
					<div class="absolute top-[70%] left-1/2 -translate-1/2 transform">&#x275D;</div>
				</div>
				<p class="sm:text-normal text-sm">
					At Ceema Eagles Academy, we believe in nurturing young minds to soar to their highest potential. Our innovative approach to education combines academic rigor with practical skills, empowering students to become confident leaders and creative problem-solvers in an ever-changing world.
				</p>
			</div>
			<div class="h-auto w-full">
				<img src={image} alt="School" class="h-full w-full object-cover" />
			</div>
		</div>
		<div class="sm:text-normal space-y-16 py-5 text-sm text-[#333]">
			<p>
				Ceema Eagles Academy is a growing educational institution in Kumasi dedicated to nurturing confident,
				disciplined, and academically strong students. The school focuses on providing a solid foundation in
				literacy, numeracy, and character development while creating a safe, supportive environment for
				children to learn and thrive.
			  </p>
			
			  <p>
				With committed teachers and a structured academic system, Ceema Eagles Academy blends modern teaching
				methods with strong moral training. The school emphasizes creativity, practical learning, discipline,
				and excellence, helping students develop the skills they need for both school life and the world
				beyond. From classroom activities to extracurricular programs, every aspect of the learning
				experience is designed to unlock each child’s potential.
			  </p>
			
			  <p>
				At Ceema Eagles Academy, every student is valued, guided, and encouraged to soar higher—just like an
				eagle. The academy continues to invest in quality education, improved facilities, and innovative
				learning experiences to ensure every learner receives the best possible start in life.
			  </p>
		</div>
	</div>
</section>
