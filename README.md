# MySite3
MortisCoder-github-io
<!DOCTYPE html>
<html lang="ru">

<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Мой первый сайт</title>
	<link rel="stylesheet">
  <style>body {
	font-family: Arial, sans-serif;
	margin: 0;
	padding: 0;
	background-color: #f4f4f4;
}

header {
	background-color: #333;
	color: white;
	padding: 10px;
	text-align: center;
}

main {
	padding: 20px;
	text-align: center;
}

button {
	background-color: #4CAF50;
	color: white;
	border: none;
	padding: 10px 20px;
	text-align: center;
	text-decoration: none;
	display:inline-block;
	font-size: 16px;
	margin: 10px 2px;
	cursor: pointer;
	transition: transform 0.3s ease;
}

/* Анимация нажатия */
button:active {
	animation: press 0.3s ease forwards;
}

/* Ключевые кадры анимации */
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

header {
	font-size: 20px;
	background-color: burlywood;
	margin: 0px;
	color: wheat;
}

main {
	font-size: 30px;
	padding: 0px;
	text-align: center;
	margin: 100px 200px;
}

body {
	font-family: Arial, Helvetica, sans-serif;
	background-color: antiquewhite;
	padding: 0px;
	margin: 0px;
}

button {
	transition: all 0.3s ease;
	margin: 100px 300px;
	cursor: pointer;
	padding: 50px 100px;
	text-align: center;
	font-size: 20px;
	background-color: wheat;
	color: black
}

button:hover {
	border: 5px solid beige;

	transform: scale(1.1) rotate(5deg);

	transform: scale(1.1);

	box-shadow: 0 10px 9px rgba(0, 0, 0, 0.3);

}</style>
</head>

<body>
	<header>
		<h1>Добро пожаловать на мой сайт!</h1>
	</header>
	<main>
		<p>Это моя первая веб-страница. Я учусь создавать сайты с нуля.</p>
		<button id="myButton">Нажми меня</button>
	</main>
	<script src="mysite.js"></script>
</body>

</html>
