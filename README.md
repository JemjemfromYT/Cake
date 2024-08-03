<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Princess Hannah's Birthday Surprise</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            padding: 20px;
            margin: 0;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            background: linear-gradient(45deg, #ffcc00, #ff6666);
            color: #fff;
            position: relative;
            min-height: 100vh;
            overflow: auto; /* Enable vertical scrolling */
        }

        .play-button {
            padding: 10px 20px;
            background-color: #fff;
            color: #333;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
            margin-bottom: 20px;
        }

        .play-button:hover {
            background-color: #eee;
        }

        audio {
            display: none;
        }

        .cake-img {
            width: 200px;
            margin-bottom: 20px;
        }

        .leaves {
            position: absolute;
            animation: fall 10s linear infinite;
            z-index: 1;
        }

        @keyframes fall {
            0% {
                transform: translateY(-100px) rotate(0deg);
            }
            100% {
                transform: translateY(100vh) rotate(360deg);
            }
        }

        .message {
            position: absolute;
            bottom: 20px;
            font-size: 24px;
            font-weight: bold;
            z-index: 2; /* Ensure the message appears above the leaves */
        }
    </style>
</head>
<body>
    <h1>Happy Birthday Princess Hannah!</h1>

    <button class="play-button" onclick="startMusic()">Play Birthday Music 🎵</button>
    
    <audio id="birthday-music" src="link_to_birthday_music.mp3" controls></audio>
    
    <img class="cake-img" src="link_to_cake_image" alt="Birthday Cake">

    <div class="leaves">
🍃🍁
    </div>

    <div class="message">
        Wishing you a day filled with love, joy, and lots of sweet surprises! 🎉🎂🎈
    </div>

    <script>
        function startMusic() {
            const audio = document.getElementById('birthday-music');
            audio.play();
        }
    </script>
</body>
</html>
