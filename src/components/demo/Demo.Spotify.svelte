<script>

	import { autoType } from "d3";
    import WIP from "$components/helpers/WIP.svelte";
</script>

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>What We Listen</title>
</head>
    <style>
        body {
            background-color: black;
        }
        @font-face {
            font-family: 'Plein Black';
            src: url('../../styles/fonts/Plein-Black.otf') format('opentype');
            font-weight:bolder;
        }
        @font-face {
            font-family: 'Plein Bold';
            src: url('../../styles/fonts/Plein-Bold.otf') format('opentype');
            font-weight: bold;
        }
        @font-face {
            font-family: 'Plein Normal';
            src: url('../../styles/fonts/Plein-Regular.otf') format('opentype');
            font-weight: normal;
        }

        p{
            font-family: 'Plein Normal';
            color:white;
            font-size:1.5rem;
            text-align: center;
        }
        h1{
            font-family: 'Plein Black';
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
            margin:2rem auto 0rem;
        }
        h3{
            font-family: "Titania", sans-serif;
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

        iframe {
            width: 60%;
            height: 6rem;
            
            /* border-radius: 8px; */
        }
        .container {
            margin: 3rem auto;
            display: flex;
            justify-content: space-between;
        }

        .title, .graph {
            flex: 1;
            padding: 20px;
        }

        .contenedor{
            margin-top: 8rem;
        }
        .contenedor p{
            font-family: 'Plein Bold';
        }
        .contenedor iframe{
            margin: 1rem auto;
            display: flex;
            align-items: center;
            justify-items: center;
        }

    </style>
<body>
    <WIP />
    <h1>¿Qué nos dice Spotify del consumo musical actual?</h1>

    <h2>TOP 5 canciones del 2023</h2>
    <br>
    <div>
        <div id="top">
            <div>
                <iframe title="song" style="border-radius:8px;" src="https://open.spotify.com/embed/track/1BxfuPKGuaTgP7aM0Bbdwr?utm_source=generator" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
                <iframe title="song" style="border-radius:8px;" src="https://open.spotify.com/embed/track/5XeFesFbtLpXzIVDNQP22n?utm_source=generator" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
                <iframe title="song" style="border-radius:8px;" src="https://open.spotify.com/embed/track/4Dvkj6JhhA12EX05fT7y2e?utm_source=generator" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
                <iframe title="song" style="border-radius:8px;" src="https://open.spotify.com/embed/track/7MXVkk9YMctZqd1Srtv4MB?utm_source=generator" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
                <iframe title="song" style="border-radius:8px;" src="https://open.spotify.com/embed/track/1kuGVB7EU95pJObxwvfwKS?utm_source=generator" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
            </div>
        </div>
    </div>
    <br>
    <br>
    <br>
    <!-- <div class="container">
        <div class="title">
            <h3>¿Qué géneros musicales fueron populares en 2023?</h3>
            <p> En 2023 lo más escuchado fue pop</p>
        </div>
        <div class="graph">
            <iframe src='https://flo.uri.sh/visualisation/18500630/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:100%;height:600px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe>
        </div>
    </div> -->
    <div class="contenedor">
        <h2>¿Qué géneros musicales fueron populares en 2023?</h2>
        <p> En 2023 lo más escuchado fue pop</p>
        <iframe src='https://flo.uri.sh/visualisation/18500630/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:100%;height:600px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe>
    </div>
    <div class="contenedor">
        <p> La mayoría NO son explícitas</p>
        <iframe src='https://flo.uri.sh/visualisation/18501487/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:80%;height:500px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe>
    </div>
    <div class="contenedor">
        <p>Los artistas son principalmente estadounidenses</p>
        <iframe src='https://flo.uri.sh/visualisation/18501081/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:80%;height:500px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe>
    </div>
</body>
