<script>
    import Header from "../components/Header.svelte";
    import AboutUS from "../components/AboutUS.svelte";
    import Seperator from "../components/Seperator.svelte";
    import WhyChooseUS from "../components/WhyChooseUS.svelte";
    import InfoAboutUS from "../components/InfoAboutUS.svelte";
    import StudentsWellBeing from "../components/StudentsWellBeing.svelte";
    import FAQ from "../components/FAQ.svelte";

    const page ='about'
</script>

<Header {page} />
<main>
    <AboutUS />
    <Seperator />
    <WhyChooseUS />
    <InfoAboutUS />
    <StudentsWellBeing />
    <FAQ />
</main>