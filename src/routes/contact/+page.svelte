<script>
    import Header from "../components/Header.svelte";
    import ContactInfo from "../components/ContactInfo.svelte";
    import ContactForm from "../components/ContactForm.svelte";

    const page = "Contact"
</script>

<Header {page} />
<main>
    <ContactInfo />
    <ContactForm />
</main>