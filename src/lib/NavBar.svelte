<script lang="ts">
	import { onMount, afterUpdate } from 'svelte';

	let currentPageUrl = '';

	onMount(() => {
		currentPageUrl = window.location.href;
		updateNavLinks();
	});

	afterUpdate(() => {
		currentPageUrl = window.location.href;
		updateNavLinks();
	});

	function updateNavLinks() {
		const navLinks = document.querySelectorAll('.navbar li a');

		for (let i = 0; i < navLinks.length; i++) {
			const link = navLinks[i] as HTMLAnchorElement;

			if (link.href === currentPageUrl) {
				link.classList.add('font-bold');
			} else {
				link.classList.remove('font-bold');
			}
		}

		const summary = document.querySelector('#rezult');
		if (summary) {
			summary.classList.add('font-bold');
		}
	}
</script>

<header class="sticky z-10 mx-auto max-w-8xl">
	<div class="navbar bg-base-100">
		<div class="navbar-start">
			<div class="dropdown top-0">
				<!-- svelte-ignore a11y-no-noninteractive-tabindex -->
				<label tabindex="0" for="" class="btn btn-ghost lg:hidden">
					<svg
						xmlns="http://www.w3.org/2000/svg"
						class="h-5 w-5"
						fill="none"
						viewBox="0 0 24 24"
						stroke="currentColor"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="2"
							d="M4 6h16M4 12h8m-8 6h16"
						/>
					</svg>
				</label>
				<!-- svelte-ignore a11y-no-noninteractive-tabindex -->
				<ul
					tabindex="0"
					class="menu menu-sm dropdown-content mt-3 p-2 shadow rounded-box w-52 bg-base-100"
				>
					<li><a href="/">Sākums</a></li>
					<li><a href="/Grafiks">Grafiks</a></li>
					<!-- svelte-ignore a11y-no-noninteractive-tabindex -->
					<li tabindex="0">
						<details>
							<summary id="rezult">Rezultāti</summary>
							<ul class="p-2 bg-base-200">
								<li><a href="/Rezultati23">2023</a></li>
								<li><a href="/Rezultati19">2019</a></li>
								<li><a href="./rezultati18.html">2018</a></li>
								<li><a href="./rezultati17.html">2017</a></li>
								<li><a href="./rezultati16.html">2016</a></li>
							</ul>
						</details>
					</li>
					<li><a href="/Jaunumi">Jaunumi</a></li>
					<li><a href="/Galerija">Galerija</a></li>
					<li><a href="/ParMehuDienam">Par Mehu dienām</a></li>
					<li><a href="/kontakti">Kontakti</a></li>
				</ul>
			</div>
			<img src="/img/MehuLogo.png" class="h-14 w-14 rounded-full" alt="" />
			<a href="/" class="btn btn-ghost normal-case text-xl">Mehu Dienas</a>
		</div>
		<div class="navbar-center hidden lg:flex">
			<ul class="menu menu-horizontal px-1 bg-base-300 rounded-box pl-4 pr-4">
				<li><a href="/">Sākums</a></li>
				<li><a href="/Grafiks">Grafiks</a></li>
				<!-- svelte-ignore a11y-no-noninteractive-tabindex -->
				<li tabindex="0">
					<details>
						<summary id="rezult">Rezultāti</summary>
						<ul class="p-2 bg-base-200">
							<li><a href="/Rezultati23">2023</a></li>
							<li><a href="/Rezultati19">2019</a></li>
							<li><a href="./rezultati18.html">2018</a></li>
							<li><a href="./rezultati17.html">2017</a></li>
							<li><a href="./rezultati16.html">2016</a></li>
						</ul>
					</details>
				</li>
				<li><a href="/Jaunumi">Jaunumi</a></li>
				<li><a href="/Galerija">Galerija</a></li>
				<li><a href="/ParMehuDienam">Par Mehu dienām</a></li>
				<li>
					<a href="/kontakti">Kontakti</a>
				</li>
			</ul>
		</div>
		<div class="navbar-end">
			<a href="/Registracija" class="btn bg-red-600 text-white text-lg fa-bold">Reģistrācija</a>
		</div>
	</div>
</header>

<style>
	.max-w-8xl {
		max-width: 88rem;
	}
</style>
