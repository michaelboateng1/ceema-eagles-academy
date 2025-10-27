<script>
    import image1 from "$lib/assets/images/children-4768404_1280.jpg";
    import image2 from "$lib/assets/images/children-4768404_1280.jpg";
    import image3 from "$lib/assets/images/children-4768404_1280.jpg";
    import image4 from "$lib/assets/images/children-4768404_1280.jpg";


    const aboutUs = [
        {
            image: image1,
            text: "Lorem ipsum dolor sit amet consectetur."
        },
        {
            image: image2,
            text: "Lorem ipsum dolor sit amet consectetur."
        },
        {
            image: image3,
            text: "Lorem ipsum dolor sit amet consectetur."
        },
        {
            image: image4,
            text: "Lorem ipsum dolor sit amet consectetur."
        },
    ]
</script>

<section class="grid grid-cols-4 mt-60">
    {#each aboutUs as info, i}
        <div class="flex flex-col {i % 2 !== 0 ? 'flex-col-reverse' : ''}">
            <div class="w-full h-[300px]">
                <img src={info.image} alt={info.text} class="w-full h-full object-cover" />
            </div>
            <div class="w-full h-[300px] flex text-white font-semibold flex-col info-bg justify-center p-5 items-center text-center">
                <p>{info.text}</p>
            </div>
        </div>
    {/each}
</section>


<style>
    .info-bg{
        background: linear-gradient(hsla(0, 0%, 20%, .8), hsla(0, 0%, 20%, .8)), url('../../lib/assets/images/get.jpeg');
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;
        /* background-attachment: fixed; */
    }
</style>