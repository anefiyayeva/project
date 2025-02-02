  <!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Главная страница</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <a href="#content" class="skip-to-content">Перейти к основному содержимому</a>
    
    <header>
        <h1>Мой веб-сайт</h1>
        <nav>
            <ul>
                <li><a href="index.html">Главная</a></li>
                <li><a href="gallery.html">Галерея</a></li>
                <li><a href="about.html">О нас</a></li>
            </ul>
        </nav>
    </header>

    <main id="content">
        <h2>Добро пожаловать!</h2>
        <p>Это моя первая страница. Здесь находится основное содержимое.</p>
        <div class="grid">
            <img src="image1.jpg" alt="Пример изображения 1">
            <img src="image2.jpg" alt="Пример изображения 2">
        </div>
    </main>

    <footer>
        <p>&copy; 2025 Все права защищены</p>
    </footer>
</body>
</html>


/* Общие стили для всего документа */
body {
    font-family: Arial, sans-serif;
    font-size: 16px;
    margin: 0;
    padding: 0;
    background-color: #f5f5f5;
    color: #333;
}

/* Стили для ссылки "Перейти к основному содержимому" */
a.skip-to-content {
    position: absolute;
    top: -40px;
    left: 10px;
    background: #0077cc;
    color: white;
    padding: 10px;
    z-index: 100;
}

a.skip-to-content:focus {
    top: 10px;
    visibility: visible;
}

/* Стили для заголовка страницы */
header {
    background-color: #0077cc;
    color: white;
    padding: 20px;
    text-align: center;
}

/* Стили для навигационного меню */
nav {
    background-color: #005599;
    padding: 10px;
    display: flex;
    justify-content: space-around;
    align-items: center;
}

nav ul {
    list-style-type: none;
    padding: 0;
    margin: 0;
    display: flex;
}

nav ul li {
    display: inline;
    margin: 0 15px;
    width: auto;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-weight: bold;
    transition: color 0.3s;
}

nav ul li a:hover {
    color: #ffcc00;
}

nav img {
    width: 10%;
}

/* Стили для основного содержимого */
main {
    background-color: #ffffff;
    padding: 20px;
    font-size: 18px;
    max-width: 800px;
    margin: 20px auto;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    border-radius: 5px;
}

main#content {
    scroll-margin-top: 50px;
}

/* Стили для подвала страницы */
footer {
    background-color: #222;
    color: white;
    text-align: center;
    padding: 15px;
    position: relative;
    bottom: 0;
    width: 100%;
}

/* Стили для заголовков */
h1 {
    text-align: center;
    font-family: 'Georgia', serif;
    color: #0077cc;
}

/* Стили для класса grid */
.grid {
    display: grid;
    grid-template-columns: 40% 40%;
    justify-content: center;
    align-items: center;
    row-gap: 20px;
}

.grid img {
    width: 100%;
    border: 3px solid #0077cc;
    padding: 5px;
    border-radius: 10px;
}

/* Стили для flex-контейнера */
.flex {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
}

.flex img:nth-child(odd) {
    border-radius: 20px;
}

/* Стили для абзацев */
p {
    line-height: 1.6;
}
