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
        <h1 class="uppercase font-bold mb-5 text-xl sm:text-2xl text-[#e07b1c]">
          Meet our passionate faculty
        </h1>
        <p class="text-sm sm:text-normal">
          Our dedicated faculty at Ceema Eagles Academy and Smart Tribe are committed to nurturing
          curiosity, creativity, and academic excellence. From experienced teachers to skilled program
          directors, each member inspires students to explore, learn, and achieve their full potential
          in academics, coding, robotics, and abacus programs.
        </p>
      </IntroText>
      
    {#each allTeachers as teachers}
        <TeachersGroup groupFaculties={teachers.groupFacultie} groupName={teachers.groupName} />
    {/each}
</main>