<script>
    const faqs = [
    {
        question: "What programs does Ceema Eagles Academy offer?",
        answer: "We offer a variety of programs including Robotics, Coding & Programming, Abacus Training, and Smart Tribe Languages. Our curriculum is designed to foster innovation, critical thinking, and academic excellence in a supportive learning environment."
    },
    {
        question: "What are the school hours?",
        answer: "Our regular school hours are from 7:30 AM to 2:30 PM, Monday through Friday. We also offer after-school programs and extracurricular activities that may extend beyond these hours."
    },
    {
        question: "How does the admission process work?",
        answer: "Our admission process includes submission of application forms, academic records review, and an assessment test. We encourage parents and students to visit our campus for a tour and interview before finalizing enrollment."
    },
    {
        question: "What safety measures are in place for students?",
        answer: "We prioritize student safety with secure campus access, CCTV surveillance, trained security personnel, comprehensive anti-bullying programs, and regular safety drills. Our staff is trained in first aid and emergency response procedures."
    },
    {
        question: "Do you offer scholarships or financial aid?",
        answer: "Yes, we offer need-based financial aid and merit scholarships. Please contact our admissions office for specific details about eligibility and application procedures for financial assistance programs."
    },
    {
        question: "What technology is integrated into the learning experience?",
        answer: "Our classrooms are equipped with smart boards, and students have access to computer labs and tablets. We incorporate educational technology and digital literacy across our curriculum to prepare students for the modern world."
    }
];
    let currentFaq = $state(null);

    const toggleFaq = (i) => {
        currentFaq = i !== currentFaq ? i : null;
    }
</script>

<section class="container mx-auto sm:w-[800px]  sm:px-20 mb-20 mt-60">
    <h2 class="capitalize font-bold mb-10 text-center text-xl sm:text-2xl">Freaquently asked question.</h2>
    {#each faqs as faq, i}
        <div class="shadow-lg rounded-sm border-t-4 ">
            <div class="px-10 py-5 cursor-pointer text-md font-bold flex justify-between items-center" tabindex="0" role="button" onkeydown={() => toggleFaq} onclick={() => toggleFaq(i)}>
                <h2>{faq.question}</h2>
                <i class="fa-solid fa-chevron-down transform transition-all duration-300 {i === currentFaq ? 'rotate-180' : 'rotate-0'}"></i>
            </div>
            <p class="transition-all duration-300 px-10 text-sm {i === currentFaq ? "opacity-100 max-h-screen py-4" : "max-h-0 opacity-0 py-0 overflow-hidden"}">{faq.answer}</p>
        </div>
    {/each}
</section>


