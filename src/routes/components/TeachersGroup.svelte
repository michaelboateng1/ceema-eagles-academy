<script>
    import TeacherCard from "./TeacherCard.svelte";

    export let groupName;
    export let groupFaculties;
</script>

<article class="sm:px-20 px-5 py-10">
    <h2 class="uppercase font-bold mb-5 text-xl sm:text-2xl">{groupName}</h2>
    <div class="grid grid-cols-2 lg:grid-cols-4 gap-5 sm:gap-10">
        {#each groupFaculties as teacher }
            <TeacherCard {teacher} />
        {/each}
    </div>
</article>