<!-- 
<div>
	<img src='assets/img/logo.png' alt="">
</div>
<style>
	img {
		width: 40rem;
		height: auto;
		margin: auto;
	}
	div {
		position: fixed;
		z-index: 999999999;
		top: 0;
		left: 0;
		width: 100%;
		text-align: center;
		padding: 1.25em;
		background: black;
		color: var(--color-bg);
		font-family: monospace;
		font-size: 16px;
	}
</style> -->
<!-- 
	<script>
		import { onMount } from 'svelte';
		
		let scrollPosition = 0;
		
		onMount(() => {
			window.addEventListener('scroll', handleScroll);
			return () => window.removeEventListener('scroll', handleScroll);
		});
		
		function handleScroll() {
			scrollPosition = window.scrollY;
		}
		
	</script>

	<div class="logo-container">
		<img style="transform: scale({1 - (scrollPosition / 1000)});" src="assets/img/logo.png" alt="">
	</div>
	
	<style>
		.logo-container {
			position: fixed;
			z-index: 999999999;
			top: 0;
			left: 0;
			width: 100%;
			text-align: center;
			padding: 1.25em;
			background: black;
			color: var(--color-bg);
			font-family: monospace;
			font-size: 16px;
			transition: transform 0.3s ease-out; /* Añade una transición suave al escalamiento */
		}
		
		img {
			width: 40rem;
			height: auto;
			margin: auto;
		}
	</style> 
-->

<script>
import { onMount } from 'svelte';

let scrollPosition = 0;
let scaleFactor = 1;
onMount(() => {
	window.addEventListener('scroll', handleScroll);
	return () => window.removeEventListener('scroll', handleScroll);
});

function handleScroll() {
	scrollPosition = window.scrollY;
	scaleFactor = Math.max(0.4, 1 - (scrollPosition / 1000)); // Minimum scale factor set to 0.3
}
</script>

<div class="logo-container">
	<img src="assets/img/logo.png" alt="" style="transform: scale({scaleFactor});">
</div>

<style>
	.logo-container {
		position: fixed;
		z-index: 999999999;
		top: 0;
		width: 100%;
		background: black;
	}
	img {
		width: 50rem;
		margin: 1rem auto;
		transition: transform 0.1s ease-out;
	}		

</style>
