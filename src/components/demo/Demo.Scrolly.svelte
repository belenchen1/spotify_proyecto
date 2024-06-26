<!-- <script>
	import Scrolly from "$components/helpers/Scrolly.svelte";
	let value;
</script>

<section id="scrolly">
	<h2>Scrolly <span>{value}</span></h2>
	<div class="spacer" />
	<Scrolly bind:value>
		{#each [0, 1, 2, 3, 4] as text, i}
			{@const active = value === i}
			<div class="step" class:active>
				<p>{text}</p>
			</div>
		{/each}
	</Scrolly>
	<div class="spacer" />
</section>

<style>
	h2 {
		position: sticky;
		top: 4em;
	}

	.spacer {
		height: 75vh;
	}

	.step {
		height: 80vh;
		background: var(--color-gray-100);
		text-align: center;
	}

	.step p {
		padding: 1rem;
	}
</style> -->
<script>
	import Scrolly from "$components/helpers/Scrolly.svelte";
	let h1Element, pElement, imgElement;
</script>

<Scrolly bind:h1Element bind:pElement bind:imgElement>
	<h1 bind:this={h1Element}>Spotify tiene más de 100 millones de tracks</h1>
	<p bind:this={pElement}>Si cada track fuera una persona podrías llenar <b>6052</b> Movistar Arena.</p>
	<img bind:this={imgElement} src="/assets/large-crowd-applause-6250.mp3" alt="Una imagen">
</Scrolly>