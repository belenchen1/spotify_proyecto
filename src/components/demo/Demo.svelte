<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>What We Listen</title>
</head>

<div id="black-overlay" class:loaded={isLoaded}></div>
<div id="demo" class:loaded={isLoaded} style="margin-bottom: -2rem !important;">
	<img
		src="assets/img/header.png"
		style="margin:10rem auto 6rem; width:45em"
		alt=""
	/>
	<div id="timeline" class="timeline">
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
		<p style="margin: auto 10rem;">
			Desde su lanzamiento en 2008, <b style="color: --verde-spotify;">Spotify</b> se convirtió en el servicio de streaming más importante.
		</p>
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
<br>

<div class="tracks">
	<h1>Spotify tiene más de 100 millones de tracks</h1>
	<!--<p>Si cada track fuera una persona podrías llenar <b>6052</b> Movistar Arena.</p>
	 <audio bind:this={sound} src="/assets/large-crowd-applause-6250.mp3" preload="auto"></audio>
	<img src="/assets/img/ma.jpg" alt="Descripción" on:mouseover={playSound} on:mouseout={stopSound}>	  -->
	<p>Si cada track fuera...</p>
	<iframe src='https://flo.uri.sh/visualisation/18519085/embed' title='' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:110%;height:600px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe>
	<!-- <iframe src='https://flo.uri.sh/visualisation/18518651/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:100%;height:600px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe> -->
	<!-- <iframe src='https://flo.uri.sh/story/2451551/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:100%;height:600px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe> -->
	
	<!-- <div id="my-wrapper">
      <div
         class="flourish-embed"
         data-src="story/2451551"
         data-url="https://flo.uri.sh/story/2451551/embed"
         data-height="100%"
      >
         <script src="https://public.flourish.studio/resources/embed.js"></script>
      </div>
      <div>
         <a href="#story/2451551/slide-1"></a>
			<p>hola1</p>
      </div>
      <div>
         <a href="#story/2451551/slide-2"></a>
			<p>hola2</p>
      </div>
		<div>
         <a href="#story/2451551/slide-3"></a>
			<p>hola3</p>
      </div>
   </div> -->
</div> 

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
		font-family: "Plein", sans-serif;
		font-weight: normal;
		text-align: center;
		letter-spacing: 0.3px;
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
			/* margin-top: 20px; */
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
			font-family: "Plein";
			font-size: 2.8rem;
			font-weight: bolder;
		}

		.timeline p {
			font-size: 1.4em;
			margin-top: -1.2rem;
			margin-bottom: 40px;
			letter-spacing: 1.5px;
			color: rgba(255, 255, 255, 0.749);
		}

	/* ------------------------------------------------------------------ */
	.spotify h2 {
		font-family: "Titania";
		font-size: 2.5rem;
		margin: -0.6rem auto 1rem;
		background-image: url("assets/img/fondo.jpg");
		background-size: cover;
		-webkit-background-clip: text;
		background-clip: text;
		color: transparent;
		text-align: center;
	}
	.spotify p {
		font-size: 1.4em;
		margin-bottom: 0;
	}
	.spotify img{
		width: 17rem;
	}
	/* ----------------------------------------------------------------- */
	/* .tracks {
		position: relative;
	} */
	.tracks p {
		/* 
		position: absolute;
		top: 24rem; 
		left: 10rem; 
		transition: top 0.6s ease-out;
		*/
		font-family: 'Plein';
		font-weight: light !important;
		font-size: 1.2rem;
		text-align: center;
	}
	.tracks h1{
		font-family: 'Plein';
		font-weight: bolder;
		font-size: 2.3rem;
		text-align: center;
		color: white;
	}
	.tracks img{
		margin: 0.5rem auto 2rem; width: 40rem; height:auto;
	}
	/* .tracks iframe{
		position: relative;
		top: 200rem;
		left: 19.5rem;
	} */
	.tracks iframe{
		position: relative;
		left: -2.2rem;
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
		margin: 0rem auto 0rem;
		font-size: 2.5rem;
		font-family: 'Titania';
		background-image: url("assets/img/fondo2.jpg");
		background-size: cover;
		background-clip: text;
		color: transparent;
		text-align: center;
	}

	.top50 img {
		margin: 3rem auto 10rem;
		height: auto;
	}
	.top50 img:hover {
		transform: scale(1.03);
		cursor: url('/assets/img/ojo_cursor.png'), auto;;
		box-shadow: 0px 0px 20px 0px rgba(195, 227, 255, 0.619); 
	}

</style>


<script>
	import { onMount } from "svelte";

	let isLoaded = false;
	let sound;

	onMount(() => {
		 // Carga dinámica del script de Flourish Scrolly
		 const script = document.createElement('script');
		 script.src = "https://cdn.flourish.rocks/flourish-scrolly-v3.1.0.min.js";
		 script.onload = () => {
			  // Una vez cargado el script, inicializa Flourish Scrolly
			  initFlourishScrolly();
			  isLoaded = true;
		 };
		 document.head.appendChild(script);

		 // Configuración adicional
		 setTimeout(() => {
			  isLoaded = true; // Esta línea parece redundante dado el manejo de carga del script
		 }, 1400);

		 window.addEventListener('scroll', handleScroll);
		 return () => {
			  window.removeEventListener('scroll', handleScroll);
		 };
	});

	function playSound() {
		 sound.play().catch(error => console.error("Error al reproducir el sonido:", error));
	}

	function stopSound() {
		 sound.pause();
		 sound.currentTime = 0; // Reinicia el sonido al principio
	}

	// Asegúrate de definir la función handleScroll si se va a usar
	function handleScroll() {
		 // Lógica para manejar el evento de desplazamiento
	}
</script>