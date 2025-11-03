<script>
    export let stage;
    export let i;

    const {image, range, description} = stage;
</script>

<section class="bg-[#e7e6e6] rounded-lg overflow-hidden">
    <figure class="w-full h-auto relative">
        <img src={image} alt={range} class="w-full h-full object-cover" />
        <div class="absolute top-0 left-0 w-full h-full"></div>
        <figcaption class="absolute text-nowrap text-white bottom-3 left-1/2 transform -translate-x-1/2 font-bold text-lg ">{range}</figcaption>
    </figure>

    <div class="px-5 py-10 space-y-2 text-sm">
        <p>{description}</p>
        <a href={`/amission/${i}`} class="text-[#e07b1c] inline-block py-2 font-bold">Learn More</a>
    </div>
</section>

<style>
    img +div{
        background: linear-gradient(hsla(0, 0%, 39%, .0) 70%, hsla(0, 0%, 39%, .8));
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
    }
</style>