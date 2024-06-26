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

        iframe {
    width: 300px; /* Ajusta el ancho para que coincida con la altura deseada */
    height: 300px; /* Hace que el iframe sea cuadrado */
    border-radius: 8px; /* Opcional: añade bordes redondeados */
     width:100%;
}
       

        .title, .graph {
            flex: 1;
            padding: 20px;
        }

        .contenedor{
            margin-top: 8rem;
            felx-direction: row;
            display:flex;
            justify-content: space-between;
        }
        
        .contenedor iframe{
            margin: 1rem auto;
            display: block;
            align-items: left;
            justify-items: leff;
        }
          
      .texto {
         width: 45%; /* Ajusta según necesites */
         text-align: left;
         order:1;
         margin: 4rem;
      }
      .grafico {
         width: 50%; /* Ajusta según necesites */
         text-align: right;
         order:2;
      }
      .scrolly-container {
         margin-top: 4rem;
         display: flex;
         overflow-x: auto;
         -webkit-overflow-scrolling: touch; /* Mejora el desplazamiento en dispositivos táctiles */
         scroll-snap-type: x mandatory; /* Opcional: para un efecto de "snap" al desplazar */
         gap: 20px; /* Espacio entre iframes */
         width:100%;
      }

.scrolly-container > div {
    margin-top: 4rem;
    flex: 0 0 auto; /* Evita que los divs se estiren */
    display: flex; /* Asegura que los iframes estén en línea */
    gap: 20px; /* Espacio entre iframes */
}
  .contenedor:nth-child(2) {
    display: flex;
    flex-direction: row-reverse;
    justify-content: space-between;
    align-items: center;
}

    </style>
<body>

    <div class="contenedor">
           <div class="texto">
        <h2>En 2023 lo más escuchado fue pop</h2>
        <p> Aunque el pop sigue siendo el rey indiscutible en Spotify, géneros como el K-Pop y el urbano latino están ganando terreno, destacando una audiencia global diversa y en constante evolución hacia nuevas tendencias musicales.</p>

        </div>
       
         <div class="grafico">
        <iframe src='https://flo.uri.sh/visualisation/18500630/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:100%;height:600px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe>
         </div>
    </div>
    <div class="contenedor">
         <div class="texto" >
        <h2> La mayoría de las canciones NO son explícitas</h2>
        <p> Las canciones no explícitas tendieron a ser ligeramente más populares en 2023.
Sin embargo, la diferencia es mínima, indicando que el contenido explícito no es crucial para el éxito en la plataforma. Tanto las canciones explícitas como las no explícitas pueden alcanzar altos niveles de popularidad.</p>
        </div>
         <div class="grafico">
        <iframe src='https://flo.uri.sh/visualisation/18501487/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:80%;height:500px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe>
         </div>
    </div>
    <div class="contenedor">
         <div class="texto" >
        <h2>Los artistas son principalmente estadounidenses</h2>
        </div>
         <div class="grafico">
        <iframe src='https://flo.uri.sh/visualisation/18501081/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:80%;height:500px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe>
         </div>
    </div>
    <h2>Top 5 de 2023</h2>
    <div class="scrolly-container">
       <div>
                <iframe title="song" style="border-radius:8px;" src="https://open.spotify.com/embed/track/1BxfuPKGuaTgP7aM0Bbdwr?utm_source=generator" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
                <iframe title="song" style="border-radius:8px;" src="https://open.spotify.com/embed/track/5XeFesFbtLpXzIVDNQP22n?utm_source=generator" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
                <iframe title="song" style="border-radius:8px;" src="https://open.spotify.com/embed/track/4Dvkj6JhhA12EX05fT7y2e?utm_source=generator" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
                <iframe title="song" style="border-radius:8px;" src="https://open.spotify.com/embed/track/7MXVkk9YMctZqd1Srtv4MB?utm_source=generator" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
                <iframe title="song" style="border-radius:8px;" src="https://open.spotify.com/embed/track/1kuGVB7EU95pJObxwvfwKS?utm_source=generator" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
            </div>

    </div>
</body>
