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
    </style>
</head>
<body>
    <br>
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
</body>
</html>
