Jakub Hiža
Vianočná úloha - zvonce

<html lang="sk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <style>
        * {
            box-sizing: border-box;
        }

        body {
            margin: 0;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background: #D3D3D3;
            font-family: Arial, sans-serif;
        }

        .container {
            width: min(90vw, 450px);
        }

        h1 {
            color: white;
            text-align: center;
            margin-bottom: 25px;
        }

        .grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 12px;
        }

        .square {
            aspect-ratio: 1 / 1;
            border: none;
            border-radius: 12px;
            cursor: pointer;
            transition: transform 0.1s;
            touch-action: manipulation;
        }

        .square:active {
            transform: scale(0.92);
        }

        .square:nth-child(1) { background: #C8102E; }
        .square:nth-child(2) { background: #C0172A; }
        .square:nth-child(3) { background: #1E5631; }
        .square:nth-child(4) { background: #1A3D2B; }
        .square:nth-child(5) { background: #D4AF37; }
        .square:nth-child(6) { background: #6B3A1F; }
        .square:nth-child(7) { background: #0D1B2A; }
        .square:nth-child(8) { background: #C0C0C0; }
        .square:nth-child(9) { background: #FFFFFF; }
    </style>
</head>

<body>

    <div class="container">

        <div class="grid">
            <button class="square" aria-label="1" onclick="playTone(261.63)"></button>
            <button class="square" aria-label="2" onclick="playTone(293.66)"></button>
            <button class="square" aria-label="3" onclick="playTone(329.63)"></button>
            <button class="square" aria-label="4" onclick="playTone(349.23)"></button>
            <button class="square" aria-label="5" onclick="playTone(392.00)"></button>
            <button class="square" aria-label="6" onclick="playTone(440.00)"></button>
            <button class="square" aria-label="7" onclick="playTone(493.88)"></button>
            <button class="square" aria-label="8" onclick="playTone(523.25)"></button>
            <button class="square" aria-label="9" onclick="playTone(587.33)"></button>
        </div>
    </div>

    <script>
        const audio = new (window.AudioContext || window.webkitAudioContext)();

        function playTone(frequency) {
            if (audio.state === "suspended") {
                audio.resume();
            }

            const oscillator = audio.createOscillator();
            const gain = audio.createGain();

            oscillator.type = "sine";
            oscillator.frequency.value = frequency;

            gain.gain.setValueAtTime(0.3, audio.currentTime);
            gain.gain.exponentialRampToValueAtTime(
                0.001, audio.currentTime + 0.5
            );

            oscillator.connect(gain);
            gain.connect(audio.destination);

            oscillator.start();
            oscillator.stop(audio.currentTime + 0.5);
        }
    </script>

</body>
</html>
