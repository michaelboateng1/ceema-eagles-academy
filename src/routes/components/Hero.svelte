<script>
    import image1 from "$lib/assets/images/schoolLogo.jpg";
    import HeroCards from "./HeroCards.svelte";
</script>

<section class="h-screen w-full flex flex-col justify-center items-center relative">
    <div class="flex flex-col justify-center items-center">
        <div class="w-40 h-auto mb-10 rounded-lg overflow-hidden">
            <img src={image1} alt="School Logo" class="w-full h-full object-fit" />
        </div>
    
        <div class="text-white">
            <div class="flex flex-col items-center mb-5 justify-center">
                <h1 class="text-5xl font-bold mb-5 poppins-extrabold">Join <span class="text-[#e07b1c]">Ceema Eagles</span> Today.</h1>
                <p class="w-[50ch] capitalize text-center">We ensure better education for better world </p>
            </div>
            <div class="flex justify-center items-center gap-8">
                <a href="/conatct" class="py-2 px-10 rounded-4xl hover:bg-[#000] transition-colors duration-300 hover:text-white hover:border-[#000] border-2 border-[#e07b1c] bg-[#e07b1c] text-white">Conatct</a>
                <a href="admission" class="py-2 px-10 rounded-4xl transition-colors duration-300 hover:bg-[#000] hover:text-white hover:border-[#000] border-2 border-[#e07b1c] text-white">Join us</a>
            </div>
        </div>
    </div>

    <div class="flex justify-center items-center gap-8 absolute px-30 -bottom-20">
        <HeroCards />
        <HeroCards />
        <HeroCards />
    </div>
</section>

<style>
    section{
        background: linear-gradient(hsla(0, 0%, 20%, .5), hsla(0, 0%, 20%, .8)), url('../../lib/assets/images/get.jpeg');
        background-position: center;
        background-size: cover;
        background-repeat: no-repeat;
        background-attachment: fixed;
    }
</style>