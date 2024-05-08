<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tarjeta para el Día de la Madre</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            overflow: hidden;
            position: relative;
        }
        #background {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            background: linear-gradient(-45deg, #ff69b4, #ffcc5c, #ff69b4, #ffcc5c);
            background-size: 400% 400%;
            animation: gradient 15s ease infinite;
        }
        @keyframes gradient {
            0% {
                background-position: 0% 50%;
            }
            50% {
                background-position: 100% 50%;
            }
            100% {
                background-position: 0% 50%;
            }
        }
        .rose {
            position: absolute;
            width: 30px;
            height: 30px;
            background-color: #ff69b4;
            border-radius: 50%;
            opacity: 0;
            animation: bloom 5s infinite alternate;
        }
        .rose:nth-child(2) {
            width: 40px;
            height: 40px;
            animation-duration: 6s;
        }
        .rose:nth-child(3) {
            width: 50px;
            height: 50px;
            animation-duration: 7s;
        }
        .rose:nth-child(4) {
            width: 60px;
            height: 60px;
            animation-duration: 8s;
        }
        .rose:nth-child(5) {
            width: 70px;
            height: 70px;
            animation-duration: 9s;
        }
        .rose:nth-child(6) {
            width: 80px;
            height: 80px;
            animation-duration: 10s;
        }
        @keyframes bloom {
            from {
                opacity: 0;
                transform: scale(0.5);
            }
            to {
                opacity: 1;
                transform: scale(1);
            }
        }
        #card {
            width: 300px;
            background-color: #fff;
            border-radius: 10px;
            padding: 20px;
            margin: 50px auto;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            opacity: 0;
            animation: fadeIn 1s ease forwards;
        }
        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(-50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        h1 {
            color: #ff69b4;
            margin-bottom: 10px;
        }
        #heart {
            color: #ff69b4;
            font-size: 50px;
            margin-bottom: 20px;
            animation: heartbeat 1s infinite alternate;
        }
        @keyframes heartbeat {
            from {
                transform: scale(1);
            }
            to {
                transform: scale(1.1);
            }
        }
    </style>
</head>
<body>
    <div id="background">
        <div class="rose"></div>
        <div class="rose"></div>
        <div class="rose"></div>
        <div class="rose"></div>
        <div class="rose"></div>
        <div class="rose"></div>
    </div>
    <div id="card">
        <div id="heart">&hearts;</div>
        <h1>Feliz Día de la Madre</h1>
        <p>Gracias por ser la mejor madre del mundo. Te quiero mucho.</p>
    </div>
</body>
</html>
