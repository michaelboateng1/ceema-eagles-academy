<script>
    import Header from "../components/Header.svelte";
    import MeetOurTeachers from "../components/MeetOurTeachers.svelte";
    import TeachersGroup from "../components/TeachersGroup.svelte";


    import { allTeachers } from "$lib";



    const page = "Our-community"
</script>

<Header {page} />
<main>
    <MeetOurTeachers />
    {#each allTeachers as teachers}
    <TeachersGroup groupFaculties={teachers.groupFacultie} groupName={teachers.groupName} />
    {/each}
</main>