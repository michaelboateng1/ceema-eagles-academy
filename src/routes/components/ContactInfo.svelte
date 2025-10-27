<script>
    const directors = [
        {
            name: "Smart Tribe",
            role: "Coding, Abacus and Robotics Partener",
            email: "kofi@gmail.com",
            number: "026782392209"
        },
        {
            name: "Kofi Mafo",
            role: "Program Director",
            email: "kofi@gmail.com",
            number: "026782392209"
        },
        {
            name: "Kofi Mafo",
            role: "Program Director",
            email: "kofi@gmail.com",
            number: "026782392209"
        },
        {
            name: "Kofi Mafo",
            role: "Program Director",
            email: "kofi@gmail.com",
            number: "026782392209"
        }
    ]
</script>

<section class="flex justify-around gap-5 container mx-auto py-10 px-5 mt-30">
    <div class="flex flex-col justify-between">
        <div>
            <h2 class="uppercase font-bold mb-2 text-2xl text-[#e07b1c]">Contact us</h2>
            <!-- TODO:Insert a map -->
            <div class=" h-[300px] w-[400px] bg-black"></div>
        </div>

        <div>
            <h2 class="uppercase text-[#e07b1c] font-bold mb-2 text-2xl mt-10">Reach out</h2>
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