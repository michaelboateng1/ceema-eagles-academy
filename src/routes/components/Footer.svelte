<script>
    import logo from "$lib/assets/images/schoolLogo.jpg";
</script>

<section class="bg-[#636363] text-[#ccc] pt-10">
    <div class="flex justify-between items-center gap-5 container mx-auto px-10">
        <div class="w-[40ch] space-y-5">
            <div class="w-[100px] overflow-hidden rounded-full h-auto">
                <img src={logo} alt="School Logo" class="w-full h-full object-cover" />
            </div>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aspernatur dolorum alias, ad ratione ducimus debitis necessitatibus eius neque. Nobis, eligendi iure consectetur laboriosam quisquam saepe culpa quasi. Eligendi, sequi tempore?</p>
        </div>
        <div>
            <h2 class="uppercase font-bold mb-2">Quick Manu</h2>
            <!-- TODO:Add a marker to the list -->
            <ul class="space-y-2">
                <li>
                    <a href="/">Home</a>
                </li>
                <li>
                    <a href="/about">About us</a>
                </li>
                <li>
                    <a href="/contact">Contact us</a>
                </li>
                <li>
                    <a href="/programming">Our Programs</a>
                </li>
                <li>
                    <a href="/academics">Our Academics</a>
                </li>
            </ul>
        </div>
        <div>
            <h2 class="uppercase font-bold mb-2">Get in touch</h2>
            <div>
                <!-- TODO:Replace and correct the icons -->
                <a href="#"><i class="fa fa-facebook">facebook</i></a>
                <a href="#"><i class="fa fa-instagram">instagram</i></a>
                <a href="#"><i class="fa fa-linkedin">linkedin</i></a>
            </div>
            <a href="/contact" class="py-2 px-5 border-2 hover:bg-[#e07b1c] transition-colors duration-300 font-semibold border-[#e07b1c] rounded-lg inline-block mt-4">Contact us</a>
        </div>
        <div>
            <div class="bg-[#808080] rounded-lg w-[30ch] py-5 px-10">
                <h2 class="uppercase text-2xl font-bold">Want to work with us?</h2>
                <a href="/admission" class="py-2 px-5 hover:bg-[#e07b1c] transition-colors duration-300 font-semibold bg-[#000] rounded-lg inline-block  mt-4">Appy Now</a>
            </div>
        </div>
    </div>
    <div class="mt-5 border-t-2 border-[#808080] container mx-auto">
        <p class="text-center py-5">some copy right message</p>
    </div>
</section>

