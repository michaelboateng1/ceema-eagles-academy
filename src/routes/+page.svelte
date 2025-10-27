<script>
    import Header from "./components/Header.svelte";
    import Hero from "./components/Hero.svelte";
    import Welcome from "./components/Welcome.svelte";
    import SVAInfo from "./components/SVAInfo.svelte";
    import Quote from "./components/Quote.svelte";
    import StudentsWellBeing from "./components/StudentsWellBeing.svelte";
    import FAQ from "./components/FAQ.svelte";

    const page = 'home';
</script>

<Header {page} />
<main>
    <Hero />
    <Welcome />
    <SVAInfo />
    <Quote />
    <StudentsWellBeing />
    <FAQ />
</main>