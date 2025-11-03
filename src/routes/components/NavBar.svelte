<script>
    import Logo from "$lib/assets/images/schoolLogo.jpg"
</script>

<nav class="flex justify-between items-center py-2 px-5 sm:px-10">
    <div class=" w-15 sm:w-20 h-auto rounded-lg overflow-hidden">
        <img src={Logo} alt="School Logo" class="w-full h-full object-cover">
    </div>
    <ul class="hidden sm:flex gap-5 justify-center font-semibold items-center">
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

    <div class="w-[40px] h-[40px] flex flex-col justify-center">
        <div class="h-[4px] w-full relative bg-[#e07b1c] rounded-lg before:content-[' '] before:w-full before:h-[4px] before:bg-[#e07b1c] before:block before:absolute before:-top-3 before:left-0 before:rounded-lg after:content-[' '] after:w-full after:h-[4px] after:bg-[#e07b1c] after:block after:absolute after:-bottom-3 after:left-0 after:rounded-lg"></div>
    </div>
</nav>
