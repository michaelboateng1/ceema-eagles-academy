<script>
    export let teacher;
</script>

<section class="bg-[#e7e6e6] rounded-lg p-4">
        <div class="w-full sm:h-[200px] h-20">
            <img src={teacher.image} alt={teacher.name} class="w-full h-full object-cover" />
        </div>
    <h2 class="capitalize font-bold text-md sm:text-lg text-[#e07b1c] p-2">{teacher.name}</h2>
    <p class="text-sm uppercase text-[#333] px-2">{teacher.role}</p>
</section>
