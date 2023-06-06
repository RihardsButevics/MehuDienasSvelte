<script>
	import NavBar from '$lib/NavBar.svelte';
	import Footer from '$lib/Footer.svelte';
</script>

<NavBar />
<div class="max-w-6xl items-center mx-auto">
	<div class="p-5 bg-base-300 rounded-box m-5 text-center">
		<div class="text-2xl font-bold">Kontakti</div>

		<div class="grid grid-cols-2">
			<div class="row-span-2 pr-5 text-right font-bold">Informatīvie tālruņi:</div>
			<div class="text-left">
				<div>+371 26 351 747</div>
				<div>+371 26 961 220</div>
			</div>
		</div>
		<div class="divider" />
		<div class="grid grid-cols-2">
			<div class="row-span-2 text-right font-bold pr-5">REKVIZĪTI:</div>
			<div class="text-left">
				<div>BIEDRĪBA „TEHNISKĀS FAKULTĀTES STUDĒJOŠO PAŠPĀRVALDE”</div>
				<div>REĢISTRĀCIJAS NUMURS: 40008235553</div>
				<div>BANKA: SWEDBANKA AS</div>
				<div>KONTS: LV89HABA0551039870459</div>
				<div>BANKAS KODS: HABALV22</div>
			</div>
		</div>
		<div />
	</div>
	<div class="grid lg:grid-cols-2 grid-cols-1">
		<div class="p-5 bg-base-300 rounded-box m-5 text-center">
			<div class="text-xl font-bold">TEHNISKĀ FAKULTĀTE</div>
			<div>Jāņa Čakstes bulvāris, Jelgava, LV-3001</div>
		</div>
		<div class=" m-5">
			<div class=" ">
				<div class="">
					<iframe
						title=""
						src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2193.3181812056982!2d23.72829377719952!3d56.65158802240775!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x46ef255ab2e90e79%3A0xd4f4b2f8e4fa663!2sFaculty%20of%20Engineering!5e0!3m2!1sen!2slv!4v1685900977322!5m2!1sen!2slv"
						class="h-72 w-full border-0 rounded-lg shadow-lg"
						allow="fullscreen"
						loading="lazy"
					/>
				</div>
			</div>
		</div>
		<div class="p-5 bg-base-300 rounded-box m-5 text-center">
			<div class="text-xl font-bold">SPORTA UN ATPŪTAS KOMPLEKS “RULLĪTIS”</div>
			<div>Aku ceļš 1, Jelgava, LV-3008</div>
		</div>
		<div class=" m-5">
			<div class=" ">
				<div class="">
					<iframe
						title=""
						src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2196.3907809726434!2d23.685754926953127!3d56.59875049999997!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x46ef3bd95e4abe6d%3A0xdc4200e3a7ae823d!2sKartodroms%20%22Rull%C4%ABtis%22!5e0!3m2!1sen!2slv!4v1685901262259!5m2!1sen!2slv"
						class="h-72 w-full border-0 rounded-lg shadow-lg"
						allow="fullscreen"
						loading="lazy"
					/>
				</div>
			</div>
		</div>
	</div>
</div>

<Footer />
