<script>
	import NavBar from '$lib/NavBar.svelte';
	import Footer from '$lib/Footer.svelte';
</script>

<NavBar />

<div class="grid lg:grid-cols-3 grid-cols-1 p-5 max-w-6xl mx-auto">
	<div class="col-span-2">
		<div class="divider text-2xl">27. Aprīlis</div>
		<div class="grid h-fit card bg-base-300 rounded-box place-items-start">
			<table class="table table-zebra w-full">
				<colgroup>
					<col style="width: 20%;" />
					<col style="width: 80%;" />
				</colgroup>
				<tr>
					<td class="text-center">18:00 - 19:00</td>
					<td class="text-left">Reģistrācija auto orientēšanai</td>
				</tr>
				<tr>
					<td class="text-center">19:00 - 02:00</td>
					<td>Nakts auto orientēšanās</td>
				</tr>
			</table>
		</div>
		<div class="divider text-2xl">28. Aprīlis</div>
		<div class="grid h-fit card bg-base-300 rounded-box place-items-start">
			<table class="table table-zebra w-full">
				<colgroup>
					<col style="width: 20%;" />
					<col style="width: 80%;" />
				</colgroup>
				<tr>
					<td class="text-center">08.30</td>
					<td>Pulcēšanās pie 5.dienesta viesnīcas</td>
				</tr>
				<tr>
					<td class="text-center">09:00 - 09:30</td>
					<td>Gājiens līdz Tehniskajai fakultātei</td>
				</tr>
				<tr>
					<td class="text-center">09:30 - 10:00</td>
					<td>Mehu dienu atklāšana pie Tehniskās fakultātes</td>
				</tr>
				<tr>
					<td class="text-center">10:30 - 11:30</td>
					<td>1. kursa iesvētības</td>
				</tr>
				<tr>
					<td class="text-center">12:00 - 13:00</td>
					<td>Reģistrācija veiklības braucienam</td>
				</tr>
				<tr>
					<td class="text-center">13:00 - 15:00</td>
					<td>Veiklības brauciens</td>
				</tr>
				<tr>
					<td class="text-center">14:00 - 16:00</td>
					<td>Fakultātes institūtu sagatavotās aktivitātes</td>
				</tr>
				<tr>
					<td class="text-center">13:00 - 16:00</td>
					<td>Reģistrācija dragreisam</td>
				</tr>
				<tr>
					<td class="text-center">16:00 - 20:00</td>
					<td>Dragreiss</td>
				</tr>
				<tr>
					<td class="text-center">22:00</td>
					<td>Brīvdabas kino</td>
				</tr>
			</table>
		</div>
		<div class="divider text-2xl">29. Aprīlis</div>
		<div class="grid h-fit card bg-base-300 rounded-box place-items-start">
			<table class="table table-zebra w-full">
				<colgroup>
					<col style="width: 20%;" />
					<col style="width: 80%;" />
				</colgroup>
				<tr>
					<td class="text-center">09:00 - 11:00</td>
					<td>Reģistrācija Driftam, Ātruma aplim, Decibelu dragreisam, Skaistuma konkursam</td>
				</tr>
				<tr>
					<td class="text-center">10:00 - 15:00</td>
					<td>Fakultātes institūtu sagatavotās aktivitātes</td>
				</tr>
				<tr>
					<td class="text-center">11:00 - 17:00</td>
					<td>Auto skaistuma konkurss + decibelu dragreiss</td>
				</tr>
				<tr>
					<td class="text-center">11:00 - 14:00</td>
					<td>Ātruma aplis</td>
				</tr>
				<tr>
					<td class="text-center">14:00 - 17:00</td>
					<td>Drifts</td>
				</tr>
				<tr>
					<td class="text-center">11:00 - 15:30</td>
					<td>Reģistrācija auto izdzīvošanai</td>
				</tr>
				<tr>
					<td class="text-center">17:00 - 19:30</td>
					<td>Auto izdzīvošanas šovs</td>
				</tr>
				<tr>
					<td class="text-center">19:30</td>
					<td>Sacensību uzvarētāju apbalvošana</td>
				</tr>
				<tr>
					<td class="text-center">22:00</td>
					<td>Mehu dienu 2023 noslēgums</td>
				</tr>
			</table>
		</div>
	</div>
	<div class="">
		<div class="divider text-2xl">CENAS</div>
		<!-- CENAS -->
		<div class=" flex justify-around bg-base-300 rounded-box lg:m-5 p-9">
			<div class="overflow-x-auto">
				<table class="table">
					<!-- head -->
					<thead />
					<tbody>
						<!-- row 1 -->
						<tr class="border-b-2 border-black">
							<th>Pieaugušajiem</th>
							<td>5 EUR</td>
						</tr>
						<tr class="border-b-1 border-black">
							<th>Studentiem</th>
							<td rowspan="3">3 EUR</td>
						</tr>
						<!-- row 2 -->
						<tr class="border-b-1 border-black">
							<th>Skolēniem</th>
						</tr>
						<!-- row 3 -->
						<tr class="border-b-2 border-black">
							<th>Pensionāriem</th>
						</tr>
						<tr class="border-b-1 border-black">
							<th>Jelgavas Mehiem</th>
							<td rowspan="2">Bez Maksas</td>
						</tr>
						<tr class="border-b-2 border-black">
							<th>Ar ielūgumiem</th>
						</tr>
						<tr class="border-b-2 border-black">
							<th>Stāvvieta Mašīnai</th>
							<td>5 EUR</td>
						</tr>
						<tr class="border-b-2 border-black">
							<th>Pilna Mašīna</th>
							<td>2 EUR</td>
						</tr>
						<tr class="border-b-2 border-black">
							<th>Atkārtota iebraukšana</th>
							<td>5 EUR</td>
						</tr>
					</tbody>
				</table>
			</div>
		</div>
	</div>
</div>

<Footer />
