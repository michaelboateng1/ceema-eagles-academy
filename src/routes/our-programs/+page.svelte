<script>
    import Header from "../components/Header.svelte";
    import IntroText from "../components/IntroText.svelte";
    import ProgramsCard from "../components/ProgramsCard.svelte";

    import {ourPrograms} from "$lib/index"

    const page = "Our Programs"
</script>

<Header {page} />
<main>
    <IntroText>
        <h1 class="uppercase font-bold mb-5 text-lg sm:text-2xl text-[#e07b1c]">
          Beyond the basics
        </h1>
        <p class="text-sm sm:text-normal">
          At Ceema Eagles Academy and Smart Tribe, learning goes beyond textbooks. Students explore coding,
          robotics, and abacus programs alongside traditional subjects, developing critical thinking,
          creativity, and problem-solving skills. Our holistic approach ensures every child is prepared for
          future challenges and opportunities.
        </p>
      </IntroText>
      

    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 container mx-auto px-5 sm:px-20 pb-20 gap-10 mt-20">
        {#each ourPrograms as program, i }
            <ProgramsCard {program} {i} />
        {/each}
    </div>
</main>
