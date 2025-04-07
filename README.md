<!DOCTYPE html>
<html lang="hu">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hamarosan indulunk!</title>
    <style>
        /* Alap stílusok */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }

        body, html {
            height: 100%;
            overflow: hidden;
        }

        /* Videó háttér */
        #video-background {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            z-index: -1;
        }

        /* Tartalom középre igazítva */
        .content {
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
            padding: 20px;
            background-color: rgba(0, 0, 0, 0.5); /* Átlátszó fekete réteg */
        }

        h1 {
            font-size: 3rem;
            margin-bottom: 2rem;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }

        /* Kapcsolatfelvétel gomb */
        .contact-button {
            padding: 15px 30px;
            background: #ff6b6b;
            color: white;
            border: none;
            border-radius: 50px;
            font-size: 1.2rem;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        .contact-button:hover {
            background: #ff5252;
            transform: translateY(-3px);
        }

        /* Reszponzív design (mobil optimalizálás) */
        @media (max-width: 768px) {
            h1 {
                font-size: 2rem;
            }
            .contact-button {
                padding: 12px 25px;
                font-size: 1rem;
            }
        }
    </style>
</head>
<body>
    <!-- Végtelenített háttérvideó -->
    <video id="video-background" autoplay muted loop>
        <source src="https://assets.mixkit.co/videos/preview/mixkit-tree-with-yellow-flowers-1173-large.mp4" type="video/mp4">
        <!-- Ha a videó nem tölt be, ez a szöveg jelenik meg -->
        A böngésződ nem támogatja a videó háttért.
    </video>

    <!-- Fő tartalom -->
    <div class="content">
        <h1>Nemsokára indulunk! 🚀</h1>
        <a href="#contact" class="contact-button">Kapcsolatfelvétel</a>
    </div>
</body>
</html>
