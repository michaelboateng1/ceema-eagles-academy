<script>
    import SVAInfoCard from "./SVAInfoCard.svelte";

    import icon1 from "$lib/assets/school-bus-svgrepo-com.svg";
    import icon2 from "$lib/assets/ruler-svgrepo-com.svg";
    import icon3 from "$lib/assets/easel-svgrepo-com.svg";
    import icon4 from "$lib/assets/ruler-combination-svgrepo-com.svg";


    const svaInfo = [
    {
        title: "Robotics Program",
        description: "Our cutting-edge Robotics program introduces students to engineering and programming through hands-on projects, fostering innovation and problem-solving skills.",
        icon: icon1
    },
    {
        title: "Coding & Programming",
        description: "Master the language of the future with our comprehensive programming courses, designed to develop logical thinking and technical expertise from the ground up.",
        icon: icon2
    },
    {
        title: "Abacus Training",
        description: "Enhance mental arithmetic and cognitive abilities through our proven Abacus training program, improving calculation speed and concentration.",
        icon: icon3
    },
    {
        title: "Smart Tribe Languages",
        description: "Expand your horizons with our language programs, designed to develop multilingual proficiency and cultural awareness from an early age.",
        icon: icon4
    }
]
</script>

<section class="px-10 sm:px-30 mt-60 mb-20">
    <h2 class="capitalize text-xl sm:text-2xl mb-5 sm:mb-10 font-bold">Empowering Future Innovators Through Specialized Education.</h2>
    <div class="grid grid-cols-1 sm:grid-cols-2 container mx-auto gap-8">
        {#each svaInfo as info }
            <SVAInfoCard {info} />
        {/each}
    </div>
</section>