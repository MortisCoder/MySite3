# MySite3
MortisCoder-github-io
<!DOCTYPE html>
<html lang="ru">

<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Мой первый сайт</title>
	<link rel="stylesheet">
  <style>/* Основные стили для всего тела документа */
body {
    font-family: Arial, Helvetica, sans-serif;
    background-color: antiquewhite;
    padding: 0;
    margin: 0;
}

/* Стили для заголовка */
header {
    background-color: burlywood;
    color: wheat;
    padding: 10px;
    text-align: center;
    font-size: 20px;
}

/* Стили для основного контента */
main {
    padding: 20px;
    text-align: center;
    font-size: 30px;
    margin: 100px 20px; /* Уменьшены отступы для улучшения отображения на мобильных устройствах */
}

/* Стили для контейнера кнопок и счётчика */
.button-container {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 20px;
    margin-bottom: 20px; /* Расстояние между контейнером и кнопкой сброса */
}

/* Стили для счётчика */
#counter {
    font-size: 2em;
    margin: 0 20px; /* Отступы слева и справа от счётчика */
}

/* Стили для кнопок */
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

/* Эффект при нажатии на кнопку */
button:active {
    animation: press 0.3s ease forwards;
}

/* Ключевые кадры анимации нажатия */
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

/* Стили для кнопки сброса */
#resetButton {
    font-size: 1em;
    padding: 10px 20px;
    cursor: pointer;
    margin-top: 20px;
}

/* Эффект наведения на кнопку */
button:hover {
    border: 5px solid beige;
    transform: scale(1.1) rotate(5deg);
    box-shadow: 0 10px 9px rgba(0, 0, 0, 0.3);
}

/* Медиа-запросы для мобильных устройств */
@media (max-width: 600px) {
    main {
        font-size: 20px;
        margin: 20px; /* Уменьшение отступов для мобильных устройств */
    }

    .button-container {
        flex-direction: column; /* Вертикальное размещение кнопок и счётчика */
        gap: 10px;
    }

    #counter {
        font-size: 1.5em; /* Уменьшение размера шрифта счётчика на мобильных устройствах */
        margin: 10px 0; /* Отступы сверху и снизу от счётчика */
    }

    button {
        padding: 12px 24px; /* Увеличение отступов для удобства на мобильных устройствах */
        font-size: 18px; /* Увеличение размера шрифта для лучшей видимости */
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
		<button id="myButton">Нажми меня</button>
	</main>
	<script>// Инициализация счётчика
let count = 0;

// Функция увеличения счётчика
function increaseCounter() {
	count++;
	document.getElementById('counter').textContent = count;
}

// Функция уменьшения счётчика
function decreaseCounter() {
	count--;
	document.getElementById('counter').textContent = count;
}

// Функция сброса счётчика
function resetCounter() {
	count = 0;
	document.getElementById('counter').textContent = count;
}

// Настройка обработчиков кликов на кнопки
document.getElementById('myButton').addEventListener('click', increaseCounter);
document.getElementById('myButton2').addEventListener('click', decreaseCounter);
document.getElementById('resetButton').addEventListener('click', resetCounter);
</script>
</body>

</html>
