<script>
    import image1 from "$lib/assets/images/get.jpeg";
    import image2 from "$lib/assets/images/children-1144109_1280.jpg";
</script>

<section class="container mx-auto px-5 sm:px-20 flex justify-center items-start mt-20 sm:mt-60 mb-20">
    <div class="w-[50ch] pt-20">
        <h2 class="font-bold text-xl mb-2">Lorem ipsum dolor sit amet consectetur adipisicing.</h2>
        <p class="mb-10 text-sm text-[#333]">Lorem ipsum dolor sit amet consectetur adipisicing elit. Necessitatibus quidem harum alias doloremque sequi accusantium molestiae quisquam ipsa? Atque libero, numquam incidunt blanditiis nostrum amet a veritatis? Tempore, commodi assumenda?</p>

        <a href="/contact" class="py-3 border-2 border-[#e07b1c] hover:bg-[#000] hover:text-white hover:border-[#000] transition-colors duration-300 px-5 rounded-tl-2xl rounded-br-2xl text-white font-semibold bg-[#e07b1c]">Join us</a>
    </div>

    <div class="relative w-full hidden sm:block">
        <div class=" absolute top-0 right-0 w-1/2 h-auto rounded-lg overflow-hidden">
            <img src={image1} alt="alajlka" class="w-full h-full object-cover" />
        </div>
        <div class=" absolute top-20 left-50 w-1/2 h-auto rounded-lg overflow-hidden">
            <img src={image2} alt="aklaj;a" class="w-full h-full object-cover" />
        </div>
    </div>
</section>