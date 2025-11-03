<script>
    import image1 from "$lib/assets/images/children-1144109_1280.jpg";
    import image2 from "$lib/assets/images/children-1144109_1280.jpg";
    import image3 from "$lib/assets/images/children-4768404_1280.jpg";
    import image4 from "$lib/assets/images/get.jpeg";

    const sections = [
        {
            image: image1,
            caption: "A school for children"
        },
        {
            image: image2,
            caption: "A strong fundation"
        },
        {
            image: image3,
            caption: "Progresive education"
        },
        {
            image: image4,
            caption: "The city is our campus"
        }
    ]
</script>

<section class="">
    <div class="text-center text-[#333] p-10 mt-60">
        <h2 class="uppercase font-bold mb-5 text-xl sm:text-2xl text-[#e07b1c]">Where curious minds explor, engage, and connect</h2>
        <p class="text-sm sm:text-normal">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Saepe sapiente mollitia obcaecati eligendi doloremque quod sed voluptas vero molestias temporibus vitae, voluptatum quas ad itaque rerum illum magni aliquid animi, quidem ab fugit similique eos voluptatibus! Distinctio et autem exercitationem.</p>
    </div>
    <section class="mt-20 bg-[#ebeae5] py-30 ">
        <h2 class="uppercase font-bold mb-20 text-xl sm:text-2xl text-center">Why choose Ceema Eagles</h2>
        <div class="flex flex-col justify-center gap-10 sm:gap-5 items-center">
            {#each sections as section}
                <figure>
                    <div class="w-[200px] h-[200px] sm:w-[250px] sm:h-[250px] overflow-hidden rounded-full border-10 border-white">
                        <img src={section.image} alt={section.caption} class="w-full h-full object-cover" />
                    </div>
                    <figcaption class="text-center py-5 capitalize text-md sm:text-lg font-semibold text-[#333] ">{section.caption}</figcaption>
                </figure>
            {/each}
        </div>
    </section>
</section>

<style>
    /* p{
        color: #ebeae5;
    } */
</style>