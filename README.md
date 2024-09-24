# Mi Proyecto de Control de Videos de YouTube

Este es un código que he desarrollado para controlar múltiples videos de YouTube en una página web. 
Cuando un video se reproduce, los demás se detienen automáticamente.

## Código

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Control de Videos de YouTube</title>
</head>
<body>
    <!-- Contenedores para los videos de YouTube -->
    <div id="player1"></div>
    <div id="player2"></div>

    <!-- API de YouTube -->
    <script src="https://www.youtube.com/iframe_api"></script>
    
    <script>
    var players = [];

    function onYouTubeIframeAPIReady() {
        // Crea los reproductores de YouTube
        players.push(new YT.Player('player1', {
            height: '360',
            width: '640',
            videoId: 'VIDEO_ID_1',
            events: {
                'onStateChange': onPlayerStateChange
            }
        }));

        players.push(new YT.Player('player2', {
            height: '360',
            width: '640',
            videoId: 'VIDEO_ID_2',
            events: {
                'onStateChange': onPlayerStateChange
            }
        }));
    }

    function onPlayerStateChange(event) {
        if (event.data == YT.PlayerState.PLAYING) {
            // Detiene todos los otros videos
            for (var i = 0; i < players.length; i++) {
                if (players[i] != event.target) {
                    players[i].pauseVideo();
                }
            }
        }
    }
    </script>
</body>
</html>
