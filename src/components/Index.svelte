<script>
import { onMount } from "svelte";
import Demo from "$components/demo/Demo.svelte";
import WIP from "$components/helpers/WIP.svelte";

	let isLoaded = false;
	onMount(() => {
		setTimeout(() => {
				isLoaded = true;
		}, 600);
		window.scrollTo(0, 0);
	});
</script>

<body>
	<div id="black-overlay" class:loaded={isLoaded}></div>
	<div id="idx" class:loaded={isLoaded}>
		<WIP />
		<Demo />
	</div>
</body>


<style>
	body{
		cursor: url('/assets/img/cursor.png'), auto;
	}
	#black-overlay {
			position: fixed;
			top: 0;
			left: 0;
			width: 100%;
			height: 100%;
			background-color: black;
			opacity: 1; /* Comienza completamente negro */
			transition: opacity 1s ease; /* Transición suave de opacidad */
			z-index: 9999; /* Asegura que esté encima de todo */
	}

	#idx {
		opacity: 0; /* Empieza oculto */
		transition: opacity 1s ease; /* Transición suave de opacidad */
		position: relative; /* Asegura que los hijos no se vean afectados por z-index del overlay */
		z-index: 10000; /* Asegura que esté encima del overlay */
}

	#black-overlay, #idx {
    transition: opacity 1s ease; /* Transición suave de opacidad */
}

	#black-overlay {
		opacity: 1; /* Estado inicial completamente visible */
	}

	#idx {
		opacity: 0; /* Estado inicial completamente oculto */
	}

	.loaded {
		opacity: 0; /* Estado final para #black-overlay, haciéndolo completamente transparente */
	}

	#idx.loaded {
		opacity: 1; /* Estado final para #idx, haciéndolo completamente visible */
	}
</style>
