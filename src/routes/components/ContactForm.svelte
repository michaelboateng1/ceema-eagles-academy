<script>
    let fullName, email, number, childName, message;

    let messageStatus = $state({});

    const sendEmail = async () => {
        try{
            const emailBody = {
                fullName: fullName.value,
                email: email.value,
                number: number.value,
                childName: childName.value,
                message: message.value
            }

            const options = {
                method: "POST",
                headers: {
                    "Content-Type": "application/json"
                },
                body: JSON.stringify(emailBody)
            };
            const response = await fetch("/api/email", options);

            const data = await response.json();

            messageStatus = {
					status: response.status,
					message: data.message,
					bg: response.status === 200 ? 'bg-green-500' : 'bg-red-500'
			};

            fullName.value = "";
            email.value = "";
            number.value = "";
            childName.value = "";
            message.value = "";

            setTimeout(() => (messageStatus = {}), 3400);

        }catch (err){
            console.log(err.message);
        }
    }
</script>

<section class="container mx-auto sm:px-20 px-5 py-10 mt-20 border-t-2 border-[#ccc]">
    <p
			class="rounded-lg px-5 text-center text-white transition-all duration-300 sm:px-5 mb-10 {messageStatus.status
				? 'max-h-full py-3'
				: 'max-h-0 py-0'} {messageStatus.bg}"
		>
			{messageStatus.message}
	</p>
    <form class="sm:space-y-14 space-y-10">
        <div class="flex flex-col sm:flex-row justify-between sm:items-center gap-2 sm:gap-0">
            <label for="fullname" class="text-nowrap">Full Name<span class="text-[#f00]">*</span>:</label>
            <input bind:this={fullName} class="sm:w-[70%] w-full border-2 border-[#e07b1c] focus:outline-0 focus:border-4 rounded-lg" type="text" placeholder="enter your full name..." id="fullname" name="fullName" required />
        </div>
        <div class="flex flex-col sm:flex-row justify-between sm:items-center gap-2 sm:gap-0">
            <label for="email" class="text-nowrap">Email:</label>
            <input bind:this={email} class="sm:w-[70%] w-full border-2 border-[#e07b1c] focus:outline-0 focus:border-4 rounded-lg" type="email" placeholder="enter your email..." id="email" name="email" />
        </div>
        <div class="flex flex-col sm:flex-row justify-between sm:items-center sm:gap-20 gap-2">
            <label class="text-nowrap" for="number">Phone Number<span class="text-[#f00]">*</span>:</label>
            <input bind:this={number} class="sm:w-[70%] w-full border-2 border-[#e07b1c] focus:outline-0 focus:border-4 rounded-lg" type="tel" placeholder="enter your phone number..." id="number" name="number" required />
        </div>
        <div class="flex flex-col sm:flex-row justify-between sm:items-center sm:gap-20 gap-2">
            <label class="text-nowrap" for="fullChildName">Child's Name<span class="text-[#f00]">*</span>:</label>
            <input bind:this={childName} class="sm:w-[70%] w-full border-2 border-[#e07b1c] focus:outline-0 focus:border-4 rounded-lg" type="text" placeholder="enter your full name..." id="fullChildName" name="fullChildName" required />
        </div>
        <div class="flex flex-col sm:flex-row justify-between sm:items-center sm:gap-20 gap-2">
            <label class="text-nowrap" for="message">Tell us something:</label>
            <textarea bind:this={message} class="sm:w-[70%] w-full border-2 border-[#e07b1c] focus:outline-0 focus:border-4 rounded-lg" id="message" name="message" placeholder="Type your message here..."></textarea>
        </div>
        <div class="flex flex-col sm:flex-row justify-between sm:items-center sm:gap-20 gap-2">
            <button onclick={() => sendEmail()} type="button" class="py-2 cursor-pointer hover:opacity-60 active:opacity-100 transition-all duration-300 px-5 bg-[#e07b1c] text-white font-semibold">Submit</button>
        </div>
    </form>
</section>