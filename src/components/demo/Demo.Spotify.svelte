<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Prueba de Título</title>
    <style>
        body {
            background-color: black;
        }
        h1{
         font-family: "Titania", sans-serif;
         font-size: 2.5rem;
         margin: -1rem auto 1.5rem;
         color: white; /* Esto hace que el texto sea transparente y muestre solo el fondo */
         text-align: center;
         background-color: rgba(83, 83, 83, 0.7);
         padding: 20px; /* Espaciado interno para que el fondo tenga más espacio */
         border-radius: 50px;
        }

        h2 {
            font-family: "Titania", sans-serif;
            font-size: 2.5rem;
            margin: -1rem auto 1.5rem;
            background-image: url("/assets/img/fondo.jpg"); /* Verifica que esta ruta sea correcta */
            background-size: cover;
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent; /* Esto hace que el texto sea transparente y muestre solo el fondo */
            text-align: center;
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
            height: 160px;
            border-radius: 8px;
        }
         .container {
            display: flex;
            justify-content: space-between;
         }

         .title, .graph {
            flex: 1; /* Esto hace que cada elemento ocupe la mitad del espacio disponible */
            padding: 20px; /* Añade algo de espacio alrededor del contenido */
         }
    </style>
</head>
<body>
    <br>
    <br>
    <h1>¿Qué nos dice Spotify del consumo musical actual?</h1>
    <br>
    <h2>TOP 5 canciones del 2023</h2>
    <br>
    <div>
        <div id="top">
            <div>
                <iframe title="song" style="border-radius:8px;" src="https://open.spotify.com/embed/track/1BxfuPKGuaTgP7aM0Bbdwr?utm_source=generator" width="90%" height="100" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
                <iframe title="song" style="border-radius:8px;" src="https://open.spotify.com/embed/track/5XeFesFbtLpXzIVDNQP22n?utm_source=generator" width="90%" height="100" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
                <iframe title="song" style="border-radius:8px;" src="https://open.spotify.com/embed/track/4Dvkj6JhhA12EX05fT7y2e?utm_source=generator" width="90%" height="100" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
                <iframe title="song" style="border-radius:8px;" src="https://open.spotify.com/embed/track/7MXVkk9YMctZqd1Srtv4MB?utm_source=generator" width="90%" height="100" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
                <iframe title="song" style="border-radius:8px;" src="https://open.spotify.com/embed/track/1kuGVB7EU95pJObxwvfwKS?utm_source=generator" width="90%" height="100" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
            </div>
        </div>
    </div>
    <br>
    <br>
    <br>
      <div class="container">
      <div class="title">
         <h3>¿Qué géneros musicales fueron populares en 2023?</h3>
         <p> En 2023 lo más escuchado fue pop</p>
      </div>
      <div class="graph">
         <iframe src='https://flo.uri.sh/visualisation/18500630/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:100%;height:600px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe><div style='width:100%!;margin-top:4px!important;text-align:right!important;'><a class='flourish-credit' href='https://public.flourish.studio/visualisation/18500630/?utm_source=embed&utm_campaign=visualisation/18500630' target='_top' style='text-decoration:none!important'><img alt='Made with Flourish' src='https://public.flourish.studio/resources/made_with_flourish.svg' style='width:105px!important;height:16px!important;border:none!important;margin:0!important;'> </a></div>
      </div>
      </div>
</body>
</html>
