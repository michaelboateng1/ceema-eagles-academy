<script>
    import { relevantPrograms } from "$lib";
</script>

<section class=" bg-[#ebeae5] py-20 mt-20">
    <h2 class="uppercase font-bold mb-20 text-xl sm:text-2xl text-center">Relevant Programs</h2>

    <div class="grid grid-cols-1 sm:grid-cols-3 gap-x-10 gap-y-20 container mx-auto px-5 sm:px-10">

        {#each relevantPrograms as program }
            <div class="shadow-lg">
                <h2 class="py-4 px-5 bg-[#e07b1c] text-white font-bold text-center text-lg sm:text-xl">{program.title}</h2>
                <div class="text-center px-5 py-10 text-sm">
                    <p>{program.description}</p>
                </div>
            </div>
        {/each}
    </div>
</section>