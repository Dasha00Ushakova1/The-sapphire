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
        }
        nav {
            margin: 15px 0;
        }
        nav a {
            margin: 0 15px;
            color: white;
            text-decoration: none;
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
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }
        .product img {
            width: 200px; /* Размер изображения товара */
            height: auto;
        }
        .add-to-cart {
            background-color: #007bff;
            color: white;
            border: none;
            padding: 10px;
            cursor: pointer;
            border-radius: 5px;
            transition: background-color 0.3s;
        }
        .add-to-cart:hover {
            background-color: #0056b3;
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
    <div class="container">
        <div class="product">
            <img src="пользователь должен сам выбрать изображение" alt="Ювелирное изделие 1">
            <h2>Ювелирное изделие 1</h2>
            <p>Цена: 5000 руб.</p>
            <button class="add-to-cart" onclick="addToCart()">Добавить в корзину</button>
        </div>
        <div class="product">
            <img src="пользователь должен сам выбрать изображение" alt="Ювелирное изделие 2">
            <h2>Ювелирное изделие 2</h2>
            <p>Цена: 7000 руб.</p>
            <button class="add-to-cart" onclick="addToCart()">Добавить в корзину</button>
        </div>
        <div class="product">
            <img src="пользователь должен сам выбрать изображение" alt="Ювелирное изделие 3">
            <h2>Ювелирное изделие 3</h2>
            <p>Цена: 3000 руб.</p>
            <button class="add-to-cart" onclick="addToCart()">Добавить в корзину</button>
        </div>
        <!-- Добавьте больше товаров по необходимости -->
    </div>
    <footer>
        <p>&copy; 2023 Ювелирный магазин. Все права защищены.</p>
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
