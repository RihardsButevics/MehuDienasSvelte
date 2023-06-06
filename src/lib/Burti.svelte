<script>
	import { quintOut } from 'svelte/easing';
	import { fade, draw, fly } from 'svelte/transition';
	import { expand } from './animacija.js';
	import {
		B11,
		B12,
		B21,
		B22,
		B31,
		B32,
		B41,
		B42,
		B51,
		B52,
		B61,
		B62,
		B71,
		B72,
		B81,
		B82,
		B91,
		B92,
		B101,
		B102
	} from './burti.js';

	let visible = true;

	function animatePaths() {
		visible = true;

		const toggleVisibility = () => {
			visible = !visible;
			setTimeout(toggleVisibility, 2500); // Wait for 3 seconds before toggling visibility
		};

		toggleVisibility();
	}

	animatePaths();
</script>

<div class="hero h-64">
	{#if visible}
		<svg
			width="2200"
			height="288"
			viewBox="-100 -150 2500 600"
			fill="none"
			xmlns="http://www.w3.org/2000/svg"
		>
			<g out:fade={{ duration: 1000 }} opacity="1">
				//Mmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmmm
				<path
					in:expand={{ duration: 400, delay: 1000, easing: quintOut }}
					style="stroke: #000000; fill: #000000; stroke-width: 10;"
					d={B11}
				/>
				<path in:draw={{ duration: 1000 }} style="stroke:#000000; stroke-width: 7" d={B12} />
				//EEEEEEEEEEEEEEEEEEEEEEEE111111111111111111111111
				<path
					in:expand={{ duration: 400, delay: 1200, easing: quintOut }}
					style="stroke: #000000;  stroke-width: 10;"
					d={B91}
				/>
				//EEEEEEEEEEEEEEEEEEEEEEEE111111111111111111111111
				<path
					in:expand={{ duration: 400, delay: 1200, easing: quintOut }}
					style="stroke: #000000; fill: #000000; stroke-width: 10;"
					d={B91}
				/>
				<path in:draw={{ duration: 1000 }} style="stroke:#000000; stroke-width: 7" d={B92} />
				//hhhhhhhhhhhhhhhhhhhhhhhhhhhhhhh
				<path
					in:expand={{ duration: 400, delay: 1300, easing: quintOut }}
					style="stroke: #000000; fill: #000000; stroke-width: 10;"
					d={B101}
				/>
				<path in:draw={{ duration: 1000 }} style="stroke:#000000; stroke-width: 7" d={B102} />
				//UUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUUU
				<path
					in:expand={{ duration: 400, delay: 1400, easing: quintOut }}
					style="stroke: #000000; fill: #000000; stroke-width: 10;"
					d={B21}
				/>
				<path in:draw={{ duration: 1000 }} style="stroke:#000000; stroke-width: 7" d={B22} />
				//DDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDDD
				<path
					in:expand={{ duration: 400, delay: 1500, easing: quintOut }}
					style="stroke: #000000; fill: #000000; stroke-width: 10;"
					d={B31}
				/>
				<path in:draw={{ duration: 1000 }} style="stroke:#000000; stroke-width: 7" d={B32} />
				//iiiiiiiiiiiiiiiiiiiiiiiiiiiiii
				<path
					in:expand={{ duration: 400, delay: 1600, easing: quintOut }}
					style="stroke: #000000; fill: #000000; stroke-width: 10;"
					d={B81}
				/>
				<path in:draw={{ duration: 1000 }} style="stroke:#000000; stroke-width: 7" d={B82} />
				//EEEEEEEEEEEEEEEEEEEEE22222222222222222222222
				<path
					in:expand={{ duration: 400, delay: 1700, easing: quintOut }}
					style="stroke: #000000; fill: #000000; stroke-width: 10;"
					d={B41}
				/>
				<path in:draw={{ duration: 1000 }} style="stroke:#000000; stroke-width: 7" d={B42} />
				//NNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNNN
				<path
					in:expand={{ duration: 400, delay: 1800, easing: quintOut }}
					style="stroke: #000000; fill: #000000; stroke-width: 10;"
					d={B51}
				/>
				<path in:draw={{ duration: 1000 }} style="stroke:#000000; stroke-width: 7" d={B52} />

				//AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA
				<path
					in:expand={{ duration: 400, delay: 1900, easing: quintOut }}
					style="stroke: #000000; fill: #000000; stroke-width: 10;"
					d={B71}
				/>
				<path in:draw={{ duration: 1000 }} style="stroke:#000000; stroke-width: 7" d={B72} />

				//SSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSSS
				<path
					in:expand={{ duration: 400, delay: 2000, easing: quintOut }}
					style="stroke: #000000; fill: #000000; stroke-width: 10;"
					d={B61}
				/>
				<path in:draw={{ duration: 1000 }} style="stroke:#000000; stroke-width: 7" d={B62} />
			</g>
		</svg>
	{/if}
</div>

<label>
	<input type="checkbox" hidden bind:checked={visible} />
</label>

<link href="https://fonts.googleapis.com/css?family=Overpass:100,400" rel="stylesheet" />

<style>
	svg {
		width: 100%;
		height: 100%;
	}

	path {
		opacity: 1;
		fill: none;
	}

	label {
		position: absolute;
		top: 1em;
		left: 1em;
	}
</style>
