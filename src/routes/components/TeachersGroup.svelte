<script>
    import TeacherCard from "./TeacherCard.svelte";

    export let groupName;
    export let groupFaculties;

    console.log(groupName)
    console.log(groupFaculties);
</script>

<article class="px-20 py-10">
    <h2 class="uppercase font-bold mb-5 text-2xl">{groupName}</h2>
    <div class="grid grid-cols-4 gap-10">
        {#each groupFaculties as teacher }
            <TeacherCard {teacher} />
        {/each}
    </div>
</article>