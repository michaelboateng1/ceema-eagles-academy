<script>
    import Header from "../components/Header.svelte";
    import IntroText from "../components/IntroText.svelte";
    import TeachersGroup from "../components/TeachersGroup.svelte";


    import { allTeachers } from "$lib";



    const page = "Our-community"
</script>

<Header {page} />
<main>
    <IntroText>
        <h1 class="uppercase font-bold mb-5 text-2xl text-[#e07b1c]">Meet our passionate faculty</h1>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Saepe sapiente mollitia obcaecati eligendi doloremque quod sed voluptas vero molestias temporibus vitae, voluptatum quas ad itaque rerum illum magni aliquid animi, quidem ab fugit similique eos voluptatibus! Distinctio et autem exercitationem.</p>
    </IntroText>
    {#each allTeachers as teachers}
    <TeachersGroup groupFaculties={teachers.groupFacultie} groupName={teachers.groupName} />
    {/each}
</main>