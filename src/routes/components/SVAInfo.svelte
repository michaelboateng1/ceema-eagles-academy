<script>
    import SVAInfoCard from "./SVAInfoCard.svelte";

    import icon1 from "$lib/assets/school-bus-svgrepo-com.svg";
    import icon2 from "$lib/assets/ruler-svgrepo-com.svg";
    import icon3 from "$lib/assets/easel-svgrepo-com.svg";
    import icon4 from "$lib/assets/ruler-combination-svgrepo-com.svg";


    const svaInfo = [
        {
            title: "Our Transport System",
            description: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eum repudiandae esse quo molestiae voluptatem minus quisquam nesciunt unde odio rem.",
            icon: icon1
        },
        {
            title: "Our Education System",
            description: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eum repudiandae esse quo molestiae voluptatem minus quisquam nesciunt unde odio rem.",
            icon: icon2
        },
        {
            title: "Our Class Rooms",
            description: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eum repudiandae esse quo molestiae voluptatem minus quisquam nesciunt unde odio rem.",
            icon: icon3
        },
        {
            title: "Our Facilities",
            description: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eum repudiandae esse quo molestiae voluptatem minus quisquam nesciunt unde odio rem.",
            icon: icon4
        }
    ]
</script>

<section class="px-10 sm:px-30 mt-60 mb-20">
    <h2 class="capitalize text-xl sm:text-2xl mb-5 sm:mb-10 font-bold">Lorem, ipsum dolor sit amet consectetur adipisicing.</h2>
    <div class="grid grid-cols-1 sm:grid-cols-2 container mx-auto gap-8">
        {#each svaInfo as info }
            <SVAInfoCard {info} />
        {/each}
    </div>
</section>