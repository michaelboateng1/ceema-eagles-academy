<section class="container mx-auto px-20 py-10 mt-20 border-t-2 border-[#ccc]">
    <form class="space-y-14">
        <div class="flex justify-between items-center">
            <label for="fullname" class="text-nowrap">Full Name<span class="text-[#f00]">*</span>:</label>
            <input class="w-[70%] border-2 border-[#e07b1c] focus:outline-0 focus:border-4 rounded-lg" type="text" placeholder="enter your full name..." id="fullname" required />
        </div>
        <div class="flex justify-between items-center">
            <label for="email" class="text-nowrap">Email:</label>
            <input class="w-[70%] border-2 border-[#e07b1c] focus:outline-0 focus:border-4 rounded-lg" type="email" placeholder="enter your email..." id="email" />
        </div>
        <div class="flex justify-between items-center gap-20">
            <label class="text-nowrap" for="number">Phone Number<span class="text-[#f00]">*</span>:</label>
            <input class="w-[70%] border-2 border-[#e07b1c] focus:outline-0 focus:border-4 rounded-lg" type="tel" placeholder="enter your phone number..." id="number" required />
        </div>
        <div class="flex justify-between items-center gap-20">
            <label class="text-nowrap" for="fullname">Child's Name<span class="text-[#f00]">*</span>:</label>
            <input class="w-[70%] border-2 border-[#e07b1c] focus:outline-0 focus:border-4 rounded-lg" type="text" placeholder="enter your full name..." id="fullname" required />
        </div>
        <div class="flex justify-between items-center gap-20">
            <label class="text-nowrap" for="message">Tell us something:</label>
            <textarea class="w-[70%] border-2 border-[#e07b1c] focus:outline-0 focus:border-4 rounded-lg" id="message" placeholder="Type your message here..."></textarea>
        </div>
        <div class="flex justify-between items-center gap-20">
            <button type="submit" class="py-2 cursor-pointer hover:opacity-60 active:opacity-100 transition-all duration-300 px-5 bg-[#e07b1c] text-white font-semibold">Submit</button>
        </div>
    </form>
</section>