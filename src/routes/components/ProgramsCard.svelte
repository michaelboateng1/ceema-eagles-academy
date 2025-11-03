<script>
    export let program;
    export let i;
</script>

<section class="flex flex-col bg-[#e7e6e6] overflow-hidden shadow-lg {i % 2 !== 0 ? 'flex-col-reverse rounded-t-lg' : 'rounded-b-lg'}">
    <div class="w-full overflow-hidden h-[200px] {i % 2 !== 0 ? 'rounded-b-lg' : 'rounded-t-lg'}">
        <img src={program.image} alt={program.title} class="w-full h-full object-cover" />
    </div>
    <div class="px-5 py-10 sm:h-[200px] border-[#e07b1c] text-sm  text-[#333] {i % 2 !== 0 ? 'rounded-t-lg border-l-4' : 'rounded-b-lg border-r-4'} ">
        <h2 class="capitalize font-bold mb-2 text-lg text-[#e07b1c]">{program.title}</h2>

        <p>{program.description}</p>
    </div>
</section>