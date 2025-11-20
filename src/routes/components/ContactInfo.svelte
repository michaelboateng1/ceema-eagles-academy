<script>
    import Map from "./Map.svelte";

    const directors = [
  {
    name: "Enoch Okyere Dadzie",
    role: "Administrator - Ceema Eagles Academy",
    email: "unknown",
    number: "unknown"
  },
  {
    name: "Kwadwo Adu-Amankwa",
    role: "Head Teacher - Ceema Eagles Academy",
    email: "unknown",
    number: "unknown"
  },
  {
    name: "Smart Tribe Ghana",
    role: "Coding, Abacus & Robotics Partner",
    email: "info@thesmartribe.com",
    number: "0205003933"
  },
  {
    name: "Isaac Kofi Maafo",
    role: "Program Director - Smart Tribe",
    email: "isaac@isaackofimaafo.com",
    number: "0558740741"
  }
];

</script>

<section class="flex flex-col sm:flex-row justify-around gap-5 container mx-auto py-10 px-5 mt-30">
    <div class="flex flex-col justify-between">
        <div>
            <h2 class="uppercase font-bold mb-2 text-2xl text-[#e07b1c]">Contact us</h2>
            <Map />
        </div>

        <div class="px-5 sm:px-0">
            <h2 class="uppercase text-[#e07b1c] font-bold mb-2 text-xl sm:text-2xl mt-10">Reach out</h2>
            <p>Kumasi, Ghana</p>
            <address>AF-067-7293</address>
            <address class="mt-5"><a href="tel:+23342092809">+23342092809</a></address>
            <address><a href="mailto:ceema@gmail.com">ceema@gmail.com</a></address>
        </div>
    </div>
    <div>
        {#each directors as director}
            <div class="space-y-10 p-5 border-[#ccc] border-b-2">
                <div>
                    <h3 class="capitalize font-bold text-2xl text-[#e07b1c]">{director.name}</h3>
                    <p class="capitalize font-bold text-lg text-[#e07b1c]">{director.role}</p>
                </div>
                <div class="flex flex-col text-sm">
                    <a href="mailto:{director.email}" class="hover:underline hover:text-[#e07b1c] transition-colors duration-300">{director.email}</a>
                    <a href="tel:{director.number}" class="hover:underline hover:text-[#e07b1c] transition-colors duration-300">{director.number}</a>
                </div>
            </div>
        {/each}
    </div>
</section>