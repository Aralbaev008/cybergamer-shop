<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CyberGame Shop - Геймерские комплектующие</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@500&display=swap');

        body {
            font-family: 'Orbitron', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #050505;
            color: #0ff;
            text-align: center;
        }
        header {
            background: #111;
            padding: 20px;
            border-bottom: 3px solid #0ff;
            box-shadow: 0 0 10px #0ff;
        }
        h1 {
            color: #0ff;
            text-shadow: 0 0 10px #0ff;
        }
        nav ul {
            list-style: none;
            padding: 0;
        }
        nav ul li {
            display: inline;
            margin: 0 15px;
        }
        nav a {
            color: #0ff;
            text-decoration: none;
            font-size: 18px;
            cursor: pointer;
            transition: 0.3s;
        }
        nav a:hover {
            color: #ff0088;
            text-shadow: 0 0 8px #ff0088;
        }
        .section {
            display: none;
            padding: 20px;
        }
        .active {
            display: block;
        }
        .product {
            background: #222;
            padding: 15px;
            margin: 15px;
            border-radius: 10px;
            display: inline-block;
            width: 250px;
            text-align: center;
            box-shadow: 0 0 10px rgba(0, 255, 255, 0.7);
            transition: 0.3s;
        }
        .product:hover {
            transform: scale(1.05);
            box-shadow: 0 0 20px rgba(0, 255, 255, 1);
        }
        .product img {
            width: 100%;
            border-radius: 10px;
        }
        .specs {
            font-size: 14px;
            color: #ccc;
        }
        button {
            background: #0ff;
            color: #0a0a0a;
            padding: 10px;
            border: none;
            cursor: pointer;
            font-size: 16px;
            border-radius: 5px;
            margin-top: 10px;
            transition: 0.3s;
            box-shadow: 0 0 10px #0ff;
        }
        button:hover {
            background: #ff0088;
            color: white;
            box-shadow: 0 0 15px #ff0088;
        }
        footer {
            margin-top: 20px;
            background: #111;
            padding: 10px;
            border-top: 3px solid #0ff;
            box-shadow: 0 0 10px #0ff;
        }
    </style>
    <script>
        function showSection(sectionId) {
            document.querySelectorAll('.section').forEach(section => {
                section.classList.remove('active');
            });
            document.getElementById(sectionId).classList.add('active');
        }
    </script>
</head>
<body onload="showSection('home')">

<header>
    <h1>🔥 CyberGame Shop 🔥</h1>
    <nav>
        <ul>
            <li><a onclick="showSection('home')">🏠 Главная</a></li>
            <li><a onclick="showSection('keyboards')">⌨ Клавиатуры</a></li>
            <li><a onclick="showSection('mice')">🖱 Мыши</a></li>
            <li><a onclick="showSection('monitors')">🖥 Мониторы</a></li>
            <li><a onclick="showSection('contact')">📞 Контакты</a></li>
        </ul>
    </nav>
</header>

<section id="home" class="section active">
    <h2>⚡ Готовые игровые ПК ⚡</h2>
    <p>Выбирайте мощные сборки для игр на максималках.</p>

    <div class="product">
        <img src="комп 1.jpg" alt="Игровой ПК">
        <h4>CyberBeast X</h4>
        <p class="specs">Intel i9 / RTX 4090 / 32GB RAM / 2TB SSD</p>
        <span class="price">1 500 000₸</span>
        <button>🛒 Купить</button>
    </div>
    <div class="product">
        <img src="комп 2.jpg" alt="Игровой ПК">
        <h4>Shadow Warrior</h4>
        <p class="specs">AMD Ryzen 9 / RX 7900 XTX / 32GB RAM</p>
        <span class="price">1 300 000₸</span>
        <button>🛒 Купить</button>
    </div>
</section>

<section id="keyboards" class="section">
    <h2>Клавиатуры</h2>
    <div class="product">
        <img src="клава 1.jpg" alt="Клавиатура">
        <h4>Razer BlackWidow</h4>
        <p>Механическая клавиатура с RGB-подсветкой.</p>
        <span class="price">35 000₸</span>
        <button>🛒 Купить</button>
    </div>
</section>

<section id="mice" class="section">
    <h2>Игровые мыши</h2>
    <div class="product">
        <img src="мыш 1.jpg" alt="Игровая мышь">
        <h4>Logitech G Pro X</h4>
        <p>Беспроводная мышь для киберспорта.</p>
        <span class="price">25 000₸</span>
        <button>🛒 Купить</button>
    </div>
</section>

<section id="monitors" class="section">
    <h2>Мониторы</h2>
    <div class="product">
        <img src="monitor1.jpg" alt="Монитор">
        <h4>MSI Optix 240Hz</h4>
        <p>Игровой монитор с частотой 240 Гц.</p>
        <span class="price">150 000₸</span>
        <button>🛒 Купить</button>
    </div>
</section>

<section id="contact" class="section">
    <h2>Свяжитесь с нами</h2>
    <p>Если у вас есть вопросы, свяжитесь с нами любым удобным способом:</p>

    <div class="contact-info">
        <p><strong>Телефон:</strong> <a href="tel:+77001234567">+7 (700) 008-08-08</a></p>
        <p><strong>Email:</strong> <a href="mailto:info@smartshop.kz">info@smartshop.kz</a></p>
        <p><strong>Адрес:</strong> ул.Байтурсынова , 15, Шымкент, Казахстан</p>
    </div>

    <form>
        <input type="text" placeholder="Ваше имя" required>
        <input type="email" placeholder="Ваш Email" required>
        <textarea placeholder="Ваше сообщение" required></textarea>
        <button type="submit">Отправить</button>
    </form>
</section>
<footer>
    <p>© 2025 CyberGame Shop. Все права защищены.</p>
</footer>

</body>
</html>
