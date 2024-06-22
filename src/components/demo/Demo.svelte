

<div id="black-overlay" class:loaded={isLoaded}></div>
<div id="demo" class:loaded={isLoaded} style="margin-bottom: -2rem !important;">
	<img
		src="assets/img/header.png"
		style="margin:10rem auto 6rem; width:45em"
		alt=""
	/>
	<div class="timeline">
		<h1>De la Radio al Streaming</h1>
		<p>La evolución del consumo de la música</p>
		<div class="timeline-container">
			<img src="assets/img/timeline/linea.png" class="linea" alt="" />
			<div class="timeline-item">
				<img src="assets/img/timeline/radio.png" alt="Radio" class="radio" />
			</div>
			<div class="timeline-item">
				<img src="assets/img/timeline/vinyl.png" alt="Vinyl" class="vinilo" />
			</div>
			<div class="timeline-item">
				<img
					src="assets/img/timeline/cassette.png"
					alt="Cassette"
					class="cassette"
				/>
			</div>
			<div class="timeline-item">
				<img src="assets/img/timeline/cd.png" alt="CD" class="cd" />
			</div>
			<div class="timeline-item">
				<img
					src="assets/img/timeline/walkman.png"
					alt="Walkman"
					class="walkman"
				/>
			</div>
			<div class="timeline-item">
				<img src="assets/img/timeline/mp3.png" alt="MP3" class="mp3" />
			</div>
		</div>
	</div>
	<div class="spotify">
		<h2>Plataformas de streaming</h2>
		<p>
			Spotify, lanzado en 2008, se ha convertido en el servicio de streaming más
			importante con el tiempo.
		</p>
		<!-- <div style="display: flex; justify-content:center; align-items:center;">
			<iframe src='https://flo.uri.sh/visualisation/18476480/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:80%;height:500px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe>
			<img src="/assets/img/subtitle_spotify.png" alt="" style='width:30%;'>
		</div>
		<div style="display: flex; justify-content:center; align-items:center;">
			<p>Casi la mitad de los usuarios son <br><b style="font-family: 'Titanium'; font-size:2rem;">Premium</b></p>
			<iframe src='https://flo.uri.sh/visualisation/18477205/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:400px;height:400px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe>
		</div> -->
		<div style="ustify-items: center; align-items: center;">
			<div>
			<div style="display: flex; justify-content:center; align-items:center;">
				<iframe src='https://flo.uri.sh/visualisation/18476480/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:80%;height:500px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe>
				<img src="/assets/img/subtitle_spotify.png" alt="" style='width:30%;'>
			</div>
			<div style="display: flex; justify-content:center; align-items:center;">
				<p>Casi la mitad de los usuarios son <br><b style="font-family: 'Titanium'; font-size:2rem;">Premium</b></p>
				<iframe src='https://flo.uri.sh/visualisation/18477205/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:400px;height:400px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe>
			</div>
		</div>
	</div>
	
		<hr>
		<div class="top50">
			<h2>¿Qué se escuchó en 2023?</h2>
			
				<a href=".\src\components\demo\Demo.Spotify.svelte"><img src="/assets/img/topglobal.jpg" alt=""></a>
				<!-- <a href="demo/spotify"><img src="/assets/img/topglobal.jpg" alt=""></a> -->
		
		</div>
	</div>
</div>

<style>
	#demo {
		max-width: calc(60rem - 4rem);
		margin: 0 auto;
		opacity: 0;
		transition: opacity 1s ease;
		position: relative;
		z-index: 10000;
	}
	
	#black-overlay,
	#demo {
		transition: opacity 1s ease;
	}
	#demo.loaded {
		opacity: 1;
	}
	
	#demo p{
		font-family: "Archivo", sans-serif;
		font-weight: lighter;
		text-align: center;
	}

/* ------------------------------------- timeline ----------------------------------- */
		.linea {
			margin: 10rem auto 1rem;
			transform: translateX(-2rem);
			width: 50%;
		}
		.timeline {
			text-align: center;
			color: white;
			margin-top: 20px;
		}

		.timeline-container {
			display: flex;
			flex-direction: column;
			align-items: center;
			position: relative;
		}

		.timeline-item {
			display: flex;
			flex-direction: column;
			align-items: center;
		}
		.timeline-item img {
			width: 18rem;
			height: auto;
			box-shadow: inset;
			position: absolute;
		}
		@keyframes rotate-hover {
			0%,
			100% {
				transform: rotate(-4deg);
			}
			50% {
				transform: rotate(4deg);
			}
		}
		.timeline-item img:hover {
			animation: rotate-hover 0.6s ease-in-out infinite alternate;
			cursor: "../statics/assets/img/cursor.png" 32 32;
		}
		.radio {
			top: 0;
			left: 4rem;
		}
		.vinilo {
			top: 25rem;
			right: 3.5rem;
		}
		.cassette {
			top: 45rem;
			left: 4rem;
			width: 20rem !important;
		}
		.cd {
			top: 60rem;
			right: 3rem;
		}
		.walkman {
			top: 75rem;
			left: 3rem;
		}
		.mp3 {
			top: 100rem;
			right: 3rem;
		}

		.timeline h1 {
			font-family: "Titania";
			font-size: 2.5em;
		}

		.timeline p {
			font-size: 1.4em;
			margin-bottom: 40px;
		}
/* ------------------------------------------------------------------ */

	.spotify h2 {
		font-family: "Titania";
		font-size: 2.5rem;
		margin: -1rem auto 1.5rem;
		background-image: url("assets/img/fondo.jpg");
		background-size: cover;
		-webkit-background-clip: text;
		background-clip: text;
		color: transparent;
		text-align: center;
	}
	.spotify p {
		font-size: 1.2em;
		margin-bottom: 0;
	}
	.spotify img{
		width: 16rem;
	}
	/* ------------------------------------------------------------------- */
	.top50 {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: start;
	}
	hr{
		margin-top: 1rem;
	}

	.top50 h2 {
		margin: 3rem auto 0rem;
		font-size: 2.5rem;
		font-family: 'Titania';
		background-image: url("assets/img/fondo2.jpg");
		background-size: cover;
		background-clip: text;
		color: transparent;
		text-align: center;
	}

	.top50 img {
		margin: 3rem auto 3rem;
		height: auto;
	}
	.top50 img:hover {
		transform: scale(1.03);
		cursor: url('/assets/img/ojo_cursor.png'), auto;;
		box-shadow: 0px 0px 20px 0px rgba(195, 227, 255, 0.619); 
	}
</style>


<script>
	import DemoLink from "$components/demo/Demo.Link.svelte";
	import DemoImg from "$components/demo/Demo.Img.svelte";
	import DemoButtonSet from "$components/demo/Demo.ButtonSet.svelte";
	import DemoRange from "$components/demo/Demo.Range.svelte";
	import DemoSelect from "$components/demo/Demo.Select.svelte";
	import DemoToggle from "$components/demo/Demo.Toggle.svelte";
	import DemoSortTable from "$components/demo/Demo.SortTable.svelte";
	import DemoSvelteElement from "$components/demo/Demo.SvelteElement.svelte";
	import DemoSvelteComponent from "$components/demo/Demo.SvelteComponent.svelte";
	import DemoFigure from "$components/demo/Demo.Figure.svelte";
	import DemoTip from "$components/demo/Demo.Tip.svelte";
	import DemoScrolly from "$components/demo/Demo.Scrolly.svelte";
	import { onMount } from "svelte";
	let isLoaded = false;
	onMount(() => {
		setTimeout(() => {
			isLoaded = true;
		}, 1400);
		window.addEventListener('scroll', handleScroll);
		return () => {
			window.removeEventListener('scroll', handleScroll);
		};
	});

</script>