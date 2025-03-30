<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Khiva Bibimaryam Hotel</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; }
        header { background-color: #8B0000; color: white; padding: 20px; font-size: 24px; }
        .container { padding: 20px; }
        .room { border: 1px solid #ddd; padding: 15px; margin: 10px; display: inline-block; }
        .contact { margin-top: 20px; }
    </style>
    <script>
        document.addEventListener("DOMContentLoaded", function () {
            const userLang = navigator.language || navigator.userLanguage;
            if (userLang.startsWith("en")) {
                document.getElementById("welcome").innerText = "Welcome to Khiva Bibimaryam!";
                document.getElementById("description").innerText = "Cozy rooms in the heart of Khiva. Book now!";
                document.getElementById("roomsTitle").innerText = "Our Rooms";
                document.getElementById("contactTitle").innerText = "Contact Us";
                document.getElementById("bookTitle").innerText = "Book Online";
                document.querySelector("input[placeholder='Имя гостя']").setAttribute("placeholder", "Guest Name");
                document.querySelector("input[placeholder='Количество гостей']").setAttribute("placeholder", "Number of Guests");
                document.querySelector("input[type='submit']").setAttribute("value", "Book Now");
            }
        });
    </script>
</head>
<body>
    <header>Khiva Bibimaryam Hotel</header>
    
    <div class="container">
        <h2 id="welcome">Добро пожаловать в Khiva Bibimaryam!</h2>
        <p id="description">Уютные номера в сердце Хивы. Забронируйте прямо сейчас!</p>
        <img src="hotel.jpg" alt="Фото гостиницы" width="80%">
        
        <h3 id="roomsTitle">Наши номера</h3>
        <div class="room">Двухместный номер (1 кровать или 2 отдельные кровати, ванная комната) - 45$ / ночь</div>
        <div class="room">Двухместный номер (1 кровать или 2 отдельные кровати, ванная комната) - 45$ / ночь</div>
        <div class="room">Двухместный номер (1 кровать или 2 отдельные кровати, ванная комната) - 45$ / ночь</div>
        <div class="room">Трехместный номер (ванная комната) - 55$ / ночь</div>
        <div class="room">Трехместный номер (ванная комната) - 55$ / ночь</div>
        
        <h3 id="contactTitle">Свяжитесь с нами</h3>
        <div class="contact">
            📞 Телефон: +998 91 433 15 39 <br>
            💬 WhatsApp: <a href="https://wa.me/998915725543">Написать в WhatsApp</a>
        </div>
        
        <h3 id="bookTitle">Забронировать онлайн</h3>
        <form>
            <input type="text" placeholder="Имя гостя" required><br><br>
            <input type="number" placeholder="Количество гостей" min="1" required><br><br>
            <input type="date" required><br><br>
            <input type="submit" value="Забронировать">
        </form>
    </div>
</body>
</html>
