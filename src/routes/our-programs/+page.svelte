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
        <h1 class="uppercase font-bold mb-5 text-2xl text-[#e07b1c]">Beyond the basics</h1>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Saepe sapiente mollitia obcaecati eligendi doloremque quod sed voluptas vero molestias temporibus vitae, voluptatum quas ad itaque rerum illum magni aliquid animi, quidem ab fugit similique eos voluptatibus! Distinctio et autem exercitationem.</p>
    </IntroText>

    <div class="grid grid-cols-3 container mx-auto px-20 pb-20 gap-10 mt-20">
        {#each ourPrograms as program, i }
            <ProgramsCard {program} {i} />
        {/each}
    </div>
</main>
