<script>
    export let info;
</script>

<section class="flex flex-col lg:flex-row justify-center gap-3 items-start">
    <div class=" w-20 h-auto">
        <img src={info.icon} alt="" class="w-full h-full object-cover">
    </div>
    <div class="pt-3">
        <h2 class="text-lg font-semibold mb-2">{info.title}</h2>
        <p class="text-sm text-[#333] lg:w-[40ch]">{info.description}</p>
        <a href="/about" class="capitalize text-[#e07b1c] block mt-2 text-sm">learn more</a>
    </div>
</section>