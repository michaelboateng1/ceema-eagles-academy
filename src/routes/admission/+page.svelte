<script>
    import Header from "../components/Header.svelte";
    import IntroText from "../components/IntroText.svelte";
    import Stages from "../components/Stages.svelte";
    import RelevantPrograms from "../components/RelevantPrograms.svelte";
    import CTA from "../components/CTA.svelte";
    
    import { ourStatges } from "$lib";

    const page = "Admission"
</script>

<Header {page} />
<main>
    <IntroText>
        <h1 class="uppercase font-bold mb-5 text-xl sm:text-2xl text-[#e07b1c]">
          Get ready for a bright future
        </h1>
        <p class="text-sm sm:text-normal">
          At Ceema Eagles Academy, we prepare learners for a future full of opportunities. With strong academics,
          dedicated teachers, and a supportive environment, students gain the confidence, discipline, and skills
          they need to excel in school and beyond. Every child is encouraged to dream big and rise higher.
        </p>
        <a href="/contact" data-sveltekit-preload-data="hover" class="capitalize font-semibold text-[#e07b1c] mt-2 inline-block">
          Contact us
        </a>
      </IntroText>
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-5 container mx-auto px-5 sm:px-10 py-20">
        {#each ourStatges as stage, i }
            <Stages {stage} {i} />
        {/each}
    </div>
    <RelevantPrograms />
    <CTA />
</main>