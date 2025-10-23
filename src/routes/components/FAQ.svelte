<script>
    const faqs = [
        {
            question: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Quia, nemo?",
            answer: "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Corrupti quasi eum soluta officiis eos nihil quibusdam, minima omnis sequi dicta amet deleniti vitae harum maxime rem reiciendis cumque ea temporibus accusantium nesciunt illo voluptates dolorem. Explicabo quasi consequuntur et magnam dolor, qui vel voluptas eligendi, itaque debitis, cupiditate eveniet nemo tempora maiores! Numquam doloremque vero, at officiis quasi sequi veritatis totam! Cupiditate expedita recusandae laborum quasi reprehenderit placeat beatae illum sunt ea sapiente, aliquid voluptas quas ipsam officia corrupti culpa maiores facere, quisquam odit pariatur ad eaque. Deserunt placeat quia inventore error, tempore maxime repellat. Voluptatem porro voluptates necessitatibus iure!"
        },
        {
            question: "Lorem ipsum dolor sit amet?",
            answer: "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quibusdam voluptatibus in neque eos, quasi dolorem perspiciatis nostrum? Error excepturi eius quasi laudantium veniam corrupti quam aspernatur voluptatem optio, vero deserunt reprehenderit minus earum rem animi quibusdam! Provident iure quos molestiae earum sed odio quibusdam, dolores in pariatur ex quidem illum."
        },
        {
            question: "Lorem, ipsum dolor?",
            answer: "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Perferendis, perspiciatis voluptas ea assumenda praesentium cum vel, earum atque voluptate reprehenderit laboriosam hic, provident nam! Vero minus maiores et odio voluptatum."
        },
        {
            question: "lorem",
            answer: "lorem, ipsum"
        },
        {
            question: "lorem",
            answer: "lorem, ipsum"
        },
        {
            question: "lorem",
            answer: "lorem, ipsum"
        },
    ]

    let currentFaq = $state(null);

    const toggleFaq = (i) => {
        currentFaq = i !== currentFaq ? i : null;
    }
</script>

<section class="container mx-auto w-[800px] px-20 mb-20 mt-60">
    <h2 class="capitalize font-bold mb-10 text-center text-2xl">Freaquently asked question.</h2>
    {#each faqs as faq, i}
        <div class="shadow-lg rounded-sm border-t-4 ">
            <div class="px-10 py-5 cursor-pointer text-md font-bold flex justify-between items-center" onclick={() => toggleFaq(i)}>
                <h2>{faq.question}</h2>
                <i class="fa-solid fa-chevron-down transform transition-all duration-300 {i === open ? 'rotate-180' : 'rotate-0'}"></i>
            </div>
            <p class="transition-all duration-300 px-10 text-sm {i === currentFaq ? "opacity-100 max-h-screen py-4" : "max-h-0 opacity-0 py-0 overflow-hidden"}">{faq.answer}</p>
        </div>
    {/each}
</section>


