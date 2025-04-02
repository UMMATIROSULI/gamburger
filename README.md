<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Abrorjon & Ominaxon larning toʻyi</title>
    <style>
        body {
            font-family: "Lucida Calligraphy", cursive;
            text-align: center;  
            background: url('https://nerminelcin.wordpress.com/wp-content/uploads/2013/05/fon.jpg') no-repeat center center fixed;
            background-size: cover;
            color: #fff;
            margin: 0;
            padding: 20px;
            position: relative;
        }
        h1 {
            font-size: 3em;
            text-shadow: 3px 3px 6px rgba(0, 0, 0, 0.7);
        }
        #countdown {
            font-size: 2.5em;
            margin: 20px 0;
            font-weight: bold;
            background: rgba(0, 0, 0, 0.5);
            display: inline-block;
            padding: 15px 25px;
            border-radius: 10px;
            white-space: pre-line;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7);
            animation: fadeIn 1s ease-in-out;
        }
        .info {
            font-size: 1.8em;
            margin: 10px 0;
            text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7);
        }
        a {
            color: #ffcc00;
            text-decoration: none;
            font-weight: bold;
            border: 2px solid #ffcc00;
            padding: 10px 20px;
            border-radius: 5px;
            transition: all 0.3s ease;
        }
        a:hover {
            background-color: #ffcc00;
            color: #000;
        }
        .share-btns {
            margin-top: 20px;
        }
        .share-btns a {
            margin: 10px;
            font-size: 1.5em;
            display: inline-block;
        }
        @media (max-width: 768px) {
            h1 { font-size: 2.5em; }
            #countdown { font-size: 2em; padding: 10px 20px; }
            .info { font-size: 1.5em; }
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
    </style>
</head>
<body>
    <h1>Abrorjon & Ominaxonning toʻyi</h1>
    <p class="info">Toʻy boshlanishiga qolgan vaqt:</p>
    <div id="countdown"></div>

    <p class="info"><strong>Sana:</strong> 2025-yil 14-aprel</p>
    <p class="info"><strong>Joy:</strong> <a href="https://yandex.ru/maps/org/31352212585?si=agjc14ekatzahgkdt1v5vpny54" target="_blank">Istiqbol, Toshkent</a></p>
    
    <p class="info"><strong>Aloqa uchun:</strong><br>
        +99899 1006007 ABRORJON<br>
        +99833 3068080 DILOROM<br>
        +99893 5555580 ANVAR<br>
    </p>

    <div class="share-btns">
        <a href="https://t.me/share/url?url=" id="telegram-share" target="_blank">Telegramda ulashish</a>
        <a href="https://calendar.google.com/calendar/r/eventedit?text=Abrorjon+%26+Ominaxonning+to'yi&dates=20250414T000000Z/20250414T050000Z&details=Istiqbol,+Toshkent&location=https://yandex.ru/maps/org/31352212585" target="_blank">Toʻyni Google Kalendariga qo‘shish</a>
    </div>

    <script>
        // Countdown timer
        function updateCountdown() {
            const weddingDate = new Date("April 14, 2025 00:00:00").getTime();
            const now = new Date().getTime();
            const timeLeft = weddingDate - now;

            const days = Math.floor(timeLeft / (1000 * 60 * 60 * 24));
            const hours = Math.floor((timeLeft % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const minutes = Math.floor((timeLeft % (1000 * 60 * 60)) / (1000 * 60));
            const seconds = Math.floor((timeLeft % (1000 * 60)) / 1000);

            document.getElementById("countdown").innerHTML = 
                `${days} kun : ${hours} soat\n${minutes} daqiqa : ${seconds} soniya`;
        }
        setInterval(updateCountdown, 1000);
        updateCountdown();

        // Dynamically update Telegram share URL
        document.getElementById('telegram-share').href = 'https://t.me/share/url?url=' + encodeURIComponent(window.location.href);
    </script>
</body>
</html>
