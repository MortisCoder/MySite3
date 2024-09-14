# MySite3
MortisCoder-github-io
<!DOCTYPE html>
<html lang="ru">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Мой первый сайт</title>
    <style>
        body {
            font-family: Arial, Helvetica, sans-serif;
            background-color: antiquewhite;
            padding: 0;
            margin: 0;
        }

        header {
            background-color: burlywood;
            color: wheat;
            padding: 10px;
            text-align: center;
            font-size: 20px;
        }

        main {
            padding: 20px;
            text-align: center;
            font-size: 30px;
            margin: 100px 20px;
        }

        .button-container {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 20px;
            margin-bottom: 20px;
        }

        #counter {
            font-size: 2em;
            margin: 0 20px;
        }

        button {
            background-color: wheat;
            color: black;
            border: none;
            padding: 10px 20px;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            margin: 10px 2px;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        button:active {
            animation: press 0.3s ease forwards;
        }

        @keyframes press {
            0% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.5);
            }
            100% {
                transform: scale(1);
            }
        }

        #resetButton {
            font-size: 1em;
            padding: 10px 20px;
            cursor: pointer;
            margin-top: 20px;
        }

        button:hover {
            border: 5px solid beige;
            transform: scale(1.1) rotate(5deg);
            box-shadow: 0 10px 9px rgba(0, 0, 0, 0.3);
        }

        @media (max-width: 600px) {
            main {
                font-size: 20px;
                margin: 20px;
            }

            .button-container {
                flex-direction: column;
                gap: 10px;
            }

            #counter {
                font-size: 1.5em;
                margin: 10px 0;
            }

            button {
                padding: 12px 24px;
                font-size: 18px;
            }
        }
    </style>
</head>

<body>
    <header>
        <h1>Добро пожаловать на мой сайт!</h1>
    </header>
    <main>
        <p>Это моя первая веб-страница. Я учусь создавать сайты с нуля.</p>
        <div class="button-container">
            <button id="myButton2">Обратно</button>
            <div id="counter">0</div>
            <button id="myButton">Дальше</button>
        </div>
        <button id="resetButton">Сбросить</button>
    </main>
    <script>
        let count = 0;

        function increaseCounter() {
            count++;
            document.getElementById('counter').textContent = count;
        }

        function decreaseCounter() {
            count--;
            document.getElementById('counter').textContent = count;
        }

        function resetCounter() {
            count = 0;
            document.getElementById('counter').textContent = count;
        }

        document.getElementById('myButton').addEventListener('click', increaseCounter);
        document.getElementById('myButton2').addEventListener('click', decreaseCounter);
        document.getElementById('resetButton').addEventListener('click', resetCounter);
    </script>
</body>

</html>
