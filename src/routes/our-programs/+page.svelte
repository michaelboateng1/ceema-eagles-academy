<script>
    import Header from "../components/Header.svelte";
    import ProgramsInfo from "../components/ProgramsInfo.svelte";
    import ProgramsCard from "../components/ProgramsCard.svelte";

    import {ourPrograms} from "$lib/index"

    const page = "Our Programs"
</script>

<Header {page} />
<main>
    <ProgramsInfo />

    <div class="grid grid-cols-3 container mx-auto px-20 pb-20 gap-10 mt-20">
        {#each ourPrograms as program, i }
            <ProgramsCard {program} {i} />
        {/each}
    </div>
</main>
