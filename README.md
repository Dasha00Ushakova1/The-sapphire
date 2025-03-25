
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ювелирный магазин</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f8f8f8;
            color: #333;
        }
        header {
            background-color: #4a4a4a;
            color: white;
            padding: 15px;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
        }
        nav {
            margin: 15px 0;
        }
        nav a {
            margin: 0 15px;
            color: white;
            text-decoration: none;
            transition: color 0.3s;
        }
        nav a:hover {
            color: #ddd;
        }
        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            padding: 20px;
        }
        .product {
            border: 1px solid #ddd;
            border-radius: 5px;
            margin: 15px;
            padding: 10px;
            text-align: center;
            background-color: white;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s, box-shadow 0.3s;
            flex: 1 1 300px; /* Для ПК-версии */
        }
        .product:hover {
            transform: scale(1.05);
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
        }
        .product img {
            width: 100%; /* Адаптивные изображения */
            height: auto;
            border-radius: 5px;
            transition: transform 0.3s;
        }
        .product img:hover {
            transform: scale(1.1);
        }
        .add-to-cart {
            background-color: #007bff;
            color: white;
            border: none;
            padding: 10px 15px;
            cursor: pointer;
            border-radius: 5px;
            transition: background-color 0.3s, transform 0.3s;
        }
        .add-to-cart:hover {
            background-color: #0056b3;
            transform: translateY(-2px);
        }
        footer {
            text-align: center;
            padding: 20px;
            background-color: #4a4a4a;
            color: white;
            position: relative;
            bottom: 0;
            width: 100%;
        }
        @media (max-width: 600px) {
            .product {
                flex: 1 1 100%; /* На маленьких экранах товары занимают всю ширину */
            }
            nav {
                display: flex;
                flex-direction: column;
                align-items: center;
            }
            nav a {
                margin: 5px 0;
            }
        }
        @media (min-width: 601px) {
            nav {
                display: flex;
                justify-content: center;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Ювелирный магазин</h1>
        <nav>
            <a href="#">Главная</a>
            <a href="#">О нас</a>
            <a href="#">Контакты</a>
            <a href="#">Корзина (<span id="cart-count">0</span>)</a>
        </nav>
    </header>
    <main class="container">
        <div class="product">
            <img src="изображение1.jpg" alt="Ювелирное изделие 1">
            <h2>Ювелирное изделие 1</h2>
            <p>Цена: 5000 руб.</p>
            <button class="add-to-cart" onclick="addToCart()">Добавить в корзину</button>
        </div>
        <div class="product">
            <img src="изображение2.jpg" alt="Ювелирное изделие 2">
            <h2>Ювелирное изделие 2</h2>
                        <p>Цена: 7000 руб.</p>
            <button class="add-to-cart" onclick="addToCart()">Добавить в корзину</button>
        </div>
        <div class="product">
            <img src="изображение3.jpg" alt="Ювелирное изделие 3">
            <h2>Ювелирное изделие 3</h2>
            <p>Цена: 3000 руб.</p>
            <button class="add-to-cart" onclick="addToCart()">Добавить в корзину</button>
        </div>
        <div class="product">
            <img src="изображение4.jpg" alt="Ювелирное изделие 4">
            <h2>Ювелирное изделие 4</h2>
            <p>Цена: 8000 руб.</p>
            <button class="add-to-cart" onclick="addToCart()">Добавить в корзину</button>
        </div>
        <div class="product">
            <img src="изображение5.jpg" alt="Ювелирное изделие 5">
            <h2>Ювелирное изделие 5</h2>
            <p>Цена: 4500 руб.</p>
            <button class="add-to-cart" onclick="addToCart()">Добавить в корзину</button>
        </div>
        <div class="product">
            <img src="изображение6.jpg" alt="Ювелирное изделие 6">
            <h2>Ювелирное изделие 6</h2>
            <p>Цена: 6500 руб.</p>
            <button class="add-to-cart" onclick="addToCart()">Добавить в корзину</button>
        </div>
    </main>
    <footer>
        <p>&copy; 2025 Ювелирный магазин Ушаковой Дарьи. Все права защищены.</p>
    </footer>
    <script>
        let cartCount = 0;
        function addToCart() {
            cartCount++;
            document.getElementById('cart-count').innerText = cartCount;
            alert("Товар добавлен в корзину!");
        }
    </script>
</body>
</html>

