<script>
	import { autoType } from "d3";
	import WIP from "$components/helpers/WIP.svelte";
</script>

<head>
	<meta charset="UTF-8" />
	<meta name="viewport" content="width=device-width, initial-scale=1.0" />
	<title>What We Listen</title>
</head>
<body>
	<div id="video" class="video-header">
		<video autoplay muted loop id="videoBackground">
			<source src="/assets/header.mp4" type="video/mp4" />
		</video>
	</div>

	<div class="contenedor">
		<div class="texto">
			<h2>Pop: ¿rey indiscutible?</h2>
			<p>
				El <b style="color: #4100f5">Pop</b> sigue dominando el escenario
				musical, pero se destaca una nueva tendencia al
				<b style="color: #cdf564">K-Pop</b>
				en particular. Sin embargo, el
				<b style="color: #9af1e1">urbano latino</b> está ganando terreno, destacando
				una audiencia global diversa.
			</p>
		</div>
		<div class="grafico">
			<iframe
				src="https://flo.uri.sh/visualisation/18500630/embed"
				title="Interactive or visual content"
				class="flourish-embed-iframe"
				frameborder="0"
				scrolling="no"
				style="width:100%;height:480px;"
				sandbox="allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation"
			></iframe>
		</div>
	</div>

	<div class="contenedor">
		<div class="texto">
			<img class="parental-advisory" src="/assets/img/explicit.png" alt=""/>
			<h2>¿Censura o Gustos?</h2>
			<p>
				Aunque las canciones no explícitas fueron un poquito más populares, el impacto de la 'censura' no marca la diferencia.
			</p>
		</div>
		<div class="grafico">
			<iframe
				src="https://flo.uri.sh/visualisation/18501487/embed"
				title="Interactive or visual content"
				class="flourish-embed-iframe"
				frameborder="0"
				scrolling="no"
				style="width:80%;height:500px;"
				sandbox="allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation"
			></iframe>
		</div>
	</div>
	<div class="contenedor">
		<div class="texto">
			<h2>¿Diversidad cultural?</h2>
			<p>
				El dominio del inglés se traduce al escenario musical: La
				mayoría de los artistas del top 50 vienen de <br> EE.UU. y el Reino Unido.
			</p>
		</div>
		<div class="grafico">
			<iframe
				src="https://flo.uri.sh/visualisation/18501081/embed"
				title="Interactive or visual content"
				class="flourish-embed-iframe"
				frameborder="0"
				scrolling="no"
				style="width:80%;height:500px;"
				sandbox="allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation"
			></iframe>
		</div>
	</div>
	<div class="scrolly-container">
		<h2>TOP 5 2023</h2>
		<div class="top5">
			<iframe
				title="song"
				style="border-radius:8px;"
				src="https://open.spotify.com/embed/track/1BxfuPKGuaTgP7aM0Bbdwr?utm_source=generator"
				frameBorder="0"
				allowfullscreen=""
				allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
				loading="lazy"
			></iframe>
			<iframe
				title="song"
				style="border-radius:8px;"
				src="https://open.spotify.com/embed/track/5XeFesFbtLpXzIVDNQP22n?utm_source=generator"
				frameBorder="0"
				allowfullscreen=""
				allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
				loading="lazy"
			></iframe>
			<iframe
				title="song"
				style="border-radius:8px;"
				src="https://open.spotify.com/embed/track/4Dvkj6JhhA12EX05fT7y2e?utm_source=generator"
				frameBorder="0"
				allowfullscreen=""
				allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
				loading="lazy"
			></iframe>
			<iframe
				title="song"
				style="border-radius:8px;"
				src="https://open.spotify.com/embed/track/7MXVkk9YMctZqd1Srtv4MB?utm_source=generator"
				frameBorder="0"
				allowfullscreen=""
				allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
				loading="lazy"
			></iframe>
			<iframe
				title="song"
				style="border-radius:8px;"
				src="https://open.spotify.com/embed/track/1kuGVB7EU95pJObxwvfwKS?utm_source=generator"
				frameBorder="0"
				allowfullscreen=""
				allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
				loading="lazy"
			></iframe>
		</div>
	</div>
</body>

<style>
	body {
		background-color: black;
	}
	@font-face {
		font-family: "Plein Black";
		src: url("../../styles/fonts/Plein-Black.otf") format("opentype");
		font-weight: bolder;
	}
	@font-face {
		font-family: "Plein Bold";
		src: url("../../styles/fonts/Plein-Bold.otf") format("opentype");
		font-weight: bold;
	}
	@font-face {
		font-family: "Plein Normal";
		src: url("../../styles/fonts/Plein-Regular.otf") format("opentype");
		font-weight: normal;
	}
	@font-face {
		font-family: 'Titania';
		src: url('./fonts/Titania.ttf') format('truetype');
	}
	p {
		font-family: "Plein Normal";
		color: white;
		font-size: 1.5rem;
		text-align: center;
	}
	h1 {
		font-family: "Plein Black";
		font-size: 2.8rem;
		font-weight: bolder;
		margin: 3rem auto 1.5rem;
		background-image: url("/assets/img/fondo.jpg");
		background-size: cover;
		-webkit-background-clip: text;
		background-clip: text;
		color: transparent;
		text-align: center;
	}

	h2 {
		font-family: "Plein Bold";
		font-size: 2.5rem;
		font-weight: normal;
		color: white;
		text-align: center;
		border-radius: 50px;
		margin: 2rem auto 0rem;
	}
	h3 {
		font-family: "Plein Bold", sans-serif;
		font-size: 2rem;
		margin: -1rem auto 1.5rem;
		color: white; /* Esto hace que el texto sea transparente y muestre solo el fondo */
		text-align: center;
	}

	#top {
		text-align: center;
	}

	#top > div {
		display: flex;
		flex-direction: column;
		align-items: center;
	}

	.title,
	.graph {
		flex: 1;
		padding: 20px;
	}

	.contenedor {
		margin-top: 8rem;
		flex-direction: row;
		display: flex;
		justify-content: space-between;
	}

	.contenedor iframe {
		margin: 1rem auto;
		display: block;
		align-items: left;
		justify-items: leff;
	}

	.texto {
		width: 45%; /* Ajusta según necesites */
		text-align: left;
		order: 1;
		/* align-items: center; */
		margin: 1rem;
	}
	.texto, .grafico {
		flex: 1; /* Hace que los elementos hijos ocupen el mismo espacio */
		display: flex;
		flex-direction: column;
		justify-content: center; /* Alinea el contenido de texto y gráfico verticalmente en el centro */
	}
	.parental-advisory {
		display: flex;
		justify-content: center;
		margin-bottom: 3rem;
		width:6rem; 
		margin: 0rem auto;
	}
	.grafico {
		width: 50%; /* Ajusta según necesites */
		text-align: right;
		order: 2;
	}
	.top5{
		display: flex;
		justify-content: space-around;
		flex-wrap: wrap;
		margin-bottom: -3rem;
	}
	.top5 iframe {
		height: 32rem;
		flex-grow: 1; /* Hace que los iframes crezcan de manera equitativa para ocupar el espacio */
		max-width: 18%; /* Establece un máximo de ancho para cada iframe */
		/* margin-bottom: -3rem !important; */
	}
	.scrolly-container h2{
		font-family: 'Titania';
		font-size: 3rem;
		letter-spacing: 4px;
		margin-bottom: 4rem;
	}

	.contenedor:nth-child(3) {
		display: flex;
		flex-direction: row-reverse;
		justify-content: space-between;
		align-items: center;
	}

	.video-header {
		position: relative;
		width: 100%;
		height: 100vh; /* Altura completa de la ventana */
		overflow: hidden;
		margin-bottom: 10rem;
	}

	#videoBackground {
		position: absolute;
		width: 100vw; /* Ancho completo de la ventana */
		height: 100vh; /* Altura completa de la ventana */
		object-fit: cover; /* Asegura que el video cubra todo el espacio */
		top: 50%;
		left: 50%;
		transform: translate(
			-50%,
			-50%
		); /* Centra el video exactamente en el medio */
	}
</style>
