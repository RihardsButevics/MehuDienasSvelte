<script>
	import NavBar from '$lib/NavBar.svelte';
	import Footer from '$lib/Footer.svelte';
	import MehuBurti from '$lib/Burti.svelte';

	// // Set the countdown date to April 25, 2024
	// const countdownDate = new Date('April 25, 2024 00:00:00').getTime();

	// // Update the countdown every second
	// const countdownTimer = setInterval(() => {
	// 	// Get the current date and time
	// 	const now = new Date().getTime();

	// 	// Calculate the time remaining until the countdown date
	// 	const timeRemaining = countdownDate - now;

	// 	// Calculate the days, hours, minutes, and seconds remaining
	// 	const days = Math.floor(timeRemaining / (1000 * 60 * 60 * 24));
	// 	const hours = Math.floor((timeRemaining % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
	// 	const minutes = Math.floor((timeRemaining % (1000 * 60 * 60)) / (1000 * 60));
	// 	const seconds = Math.floor((timeRemaining % (1000 * 60)) / 1000);

	// 	// Display the countdown values
	// 	document.getElementById('days').querySelector('.countdown').textContent = days;
	// 	document.getElementById('hours').querySelector('.countdown').textContent = hours;
	// 	document.getElementById('minutes').querySelector('.countdown').textContent = minutes;
	// 	document.getElementById('seconds').querySelector('.countdown').textContent = seconds;

	// 	// If the countdown is finished, display a message or perform any desired action
	// 	if (timeRemaining < 0) {
	// 		clearInterval(countdownTimer);
	// 		// Perform any desired action here
	// 	}
	// }, 1000);
</script>

<NavBar />

<div
	style="background-image: url(/img/MAIN_BILDE.jpg); background-position-y: 60%;"
	class="hero min-h-10"
>
	<div class="hero-overlay bg-opacity-60" />
	<div class="hero-content text-center text-neutral-content">
		<div class="">
			<MehuBurti />
		</div>
	</div>
</div>

<div class="m-auto max-w-8xl">
	<div class="flex flex-col w-full lg:flex-row p-5">
		<div class="grid flex-grow h-32 card bg-base-300 rounded-box place-items-center">
			<div class="grid grid-flow-col gap-5 text-center auto-cols-max">
				<div id="days" class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
					<span class="countdown font-mono text-5xl">
						<span style="--value:15;" />
					</span>
					days
				</div>
				<div
					id="hours"
					class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content items-center"
				>
					<span class="countdown font-mono text-5xl">
						<span style="--value:10;" />
					</span>
					hours
				</div>
				<div id="minutes" class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
					<span class="countdown font-mono text-5xl">
						<span style="--value:24;" />
					</span>
					min
				</div>
				<div id="seconds" class="flex flex-col p-2 bg-neutral rounded-box text-neutral-content">
					<span class="countdown font-mono text-5xl">
						<span style="--value:55;" />
					</span>
					sec
				</div>
			</div>
		</div>
		<div class="divider lg:divider-horizontal" />
		<div class="grid flex-grow h-32 card bg-base-300 rounded-box place-items-center">
			<div class="grid grid-flow-col gap-5 text-center auto-cols-max">
				<img src="/img/IMG_0565.jpg" class="h-24 w-auto float-left" alt="" />
				<div class="grid grid-cols-1 grid-rows-3 text-left text-xl">
					<div>25. un 26. Aprīlis</div>
					<div>Rullītis Kartingu trase</div>
					<div>Jelgava, Latvija</div>
				</div>
			</div>
		</div>
	</div>
</div>

<Footer />

<style>
	.max-w-8xl {
		max-width: 88rem;
	}
</style>
