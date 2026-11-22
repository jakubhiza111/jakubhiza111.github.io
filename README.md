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
            background: #4A4A4A;
            font-family: Arial, sans-serif;
            font
        }

        .container {
            width: min(90vw, 450px);
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

        .square:nth-child(1) { background: #FF0000; }
        .square:nth-child(2) { background: #DC143C; }
        .square:nth-child(3) { background: #8B0000; }
        .square:nth-child(4) { background: #008000; }
        .square:nth-child(5) { background: #228B22; }
        .square:nth-child(6) { background: #32CD32; }
        .square:nth-child(7) { background: #FFD700; }
        .square:nth-child(8) { background: #D4AF37; }
        .square:nth-child(9) { background: #CFB53B; }
    </style>
</head>

<body>

    <div class="container">

        <div class="grid">
            <button class="square" aria-label="1" onclick="playTone(261.63)">1</button>
            <button class="square" aria-label="2" onclick="playTone(293.66)">2</button>
            <button class="square" aria-label="3" onclick="playTone(329.63)">3</button>
            <button class="square" aria-label="4" onclick="playTone(349.23)">4</button>
            <button class="square" aria-label="5" onclick="playTone(392.00)">5</button>
            <button class="square" aria-label="6" onclick="playTone(440.00)">6</button>
            <button class="square" aria-label="7" onclick="playTone(493.88)">7</button>
            <button class="square" aria-label="8" onclick="playTone(523.25)">8</button>
            <button class="square" aria-label="9" onclick="playTone(587.33)">9</button>
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
