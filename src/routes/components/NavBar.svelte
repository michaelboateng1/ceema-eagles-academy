<script>
    import Logo from "$lib/assets/images/schoolLogo.jpg"
</script>

<nav class="flex justify-between items-center py-2 px-10">
    <div class="w-20 h-auto rounded-lg overflow-hidden">
        <img src={Logo} alt="School Logo" class="w-full h-full object-cover">
    </div>
    <ul class="flex gap-5 justify-center font-semibold items-center">
        <li>
            <a href="/" class="text-lg">Home</a>
        </li>
        <li>
            <a href="/about" class="text-lg">About</a>
        </li>
        <li>
            <a href="/contact" class="text-lg">Contact</a>
        </li>
        <li>
            <a href="/programs" class="text-lg">Programs</a>
        </li>
        <li>
            <a href="/academics" class="text-lg">Academic</a>
        </li>
    </ul>
</nav>
