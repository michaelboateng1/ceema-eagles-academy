<script>
    import Logo from "$lib/assets/images/schoolLogo.jpg";

    import mobileNav from "../store/store";

</script>

<nav class="flex justify-between items-center py-2 px-5 lg:px-10">
    <div class=" w-15 sm:w-20 h-auto rounded-lg overflow-hidden">
        <img src={Logo} alt="School Logo" class="w-full h-full object-cover">
    </div>
    <ul class="hidden lg:flex gap-5 justify-center font-semibold items-center">
        <li class="before:content-[' '] relative before:absolute before:-bottom-1 before:left-0 before:w-0 hover:before:w-full transition duration-300 before:h-[4px] before:bg-black before:block ">
            <a href="/" class="text-lg">Home</a>
        </li>
        <li>
            <a href="/about" class="text-lg">About</a>
        </li>
        <li>
            <a href="/contact" class="text-lg">Contact</a>
        </li>
        <li>
            <a href="/admission" class="text-lg">Admissions</a>
        </li>
        <li>
            <a href="/our-programs" class="text-lg">Programs</a>
        </li>
        <li>
            <a href="/our-community" class="text-lg">Our Community</a>
        </li>
    </ul>

    <div onclick={() => $mobileNav = !$mobileNav} onkeydown={() => $mobileNav = !$mobileNav} role="button" tabindex="0" class="lg:hidden w-[40px] h-[40px] flex flex-col justify-center">
        <div class="h-[4px] w-full relative bg-[#e07b1c] rounded-lg transtion-colors duration-400 before:content-[' '] before:w-full before:h-[4px] before:bg-[#e07b1c] before:block before:absolute before:-top-3 before:left-0 before:rounded-lg after:content-[' '] before:transform before:transition-transform before:duration-400 after:w-full after:h-[4px] after:bg-[#e07b1c] after:block after:absolute after:-bottom-3 after:left-0 after:rounded-lg after:transition-transform after:duration-400 after:transform {$mobileNav ? "bg-transparent before:rotate-[45deg] before:top-0 after:-rotate-[45deg] after:bottom-0" : "bg-[#e07b1c] before:rotate-[0deg] before:-top-3 after:-rotate-[0deg] after:-bottom-3"}"></div>
    </div>
</nav>
