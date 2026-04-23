<!DOCTYPE html>  
<html lang="ru">  
<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">  
    <title>Автосалон "Классика Движения" - разработка сайта</title>  
    <style>  
        * {  
            margin: 0;  
            padding: 0;  
            box-sizing: border-box;  
        }  
  
        body {  
            font-family: 'Segoe UI', 'Arial', system-ui, -apple-system, sans-serif;  
            background: #f4f7fc;  
            color: #1e2f3a;  
            line-height: 1.5;  
        }  
  
        /* Шапка */  
        .header {  
            background: #0a2f44;  
            color: white;  
            padding: 20px 0;  
            text-align: center;  
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);  
        }  
  
        .container {  
            max-width: 1200px;  
            margin: 0 auto;  
            padding: 0 20px;  
        }  
  
        .site-title {  
            font-size: 2.2rem;  
            letter-spacing: 1px;  
            margin-bottom: 8px;  
        }  
  
        .site-sub {  
            font-size: 1rem;  
            opacity: 0.85;  
        }  
  
        /* Навигация */  
        .nav {  
            background: #1c5a7a;  
            padding: 12px 0;  
            position: sticky;  
            top: 0;  
            z-index: 100;  
        }  
  
        .nav-menu {  
            display: flex;  
            justify-content: center;  
            gap: 30px;  
            flex-wrap: wrap;  
            list-style: none;  
        }  
  
        .nav-menu a {  
            color: white;  
            text-decoration: none;  
            font-weight: 500;  
            padding: 5px 0;  
            border-bottom: 2px solid transparent;  
            transition: 0.2s;  
        }  
  
        .nav-menu a:hover {  
            border-bottom-color: #ffb347;  
        }  
  
        /* Карточки машин */  
        .section {  
            padding: 50px 0;  
            border-bottom: 1px solid #dce7ed;  
        }  
  
        .section-title {  
            font-size: 2rem;  
            margin-bottom: 30px;  
            color: #0a2f44;  
            border-left: 6px solid #ff8c42;  
            padding-left: 18px;  
        }  
  
        .cars-grid {  
            display: grid;  
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));  
            gap: 30px;  
            margin-top: 20px;  
        }  
  
        .car-card {  
            background: white;  
            border-radius: 20px;  
            overflow: hidden;  
            box-shadow: 0 8px 20px rgba(0,0,0,0.08);  
            transition: transform 0.2s ease;  
        }  
  
        .car-card:hover {  
            transform: translateY(-6px);  
        }  
  
        .car-img {  
            width: 100%;  
            height: 220px;  
            object-fit: cover;  
            background: #cfdfe9;  
        }  
  
        .car-info {  
            padding: 20px;  
        }  
  
        .car-name {  
            font-size: 1.7rem;  
            font-weight: 600;  
            margin-bottom: 12px;  
            color: #1c5a7a;  
        }  
  
        .car-desc {  
            margin-bottom: 15px;  
            color: #2c4757;  
        }  
  
        .car-specs {  
            background: #eef3f8;  
            padding: 12px;  
            border-radius: 16px;  
            font-size: 0.9rem;  
            margin-top: 10px;  
        }  
  
        .story-box {  
            background: #fff9ef;  
            border-left: 6px solid #ffb347;  
            padding: 25px;  
            margin: 35px 0;  
            border-radius: 24px;  
            box-shadow: 0 4px 12px rgba(0,0,0,0.05);  
        }  
  
        footer {  
            background: #0a2f44;  
            color: #e0edf5;  
            padding: 35px 0 25px;  
            margin-top: 20px;  
        }  
  
        .footer-content {  
            display: flex;  
            flex-wrap: wrap;  
            justify-content: space-between;  
            gap: 30px;  
        }  
  
        .sources {  
            background: #001f2c;  
            padding: 15px;  
            border-radius: 24px;  
            font-size: 0.85rem;  
            margin-top: 25px;  
        }  
  
        .sources a {  
            color: #ffbc6e;  
            text-decoration: none;  
        }  
  
        .btn-like {  
            display: inline-block;  
            background: #ff8c42;  
            color: #1e2f3a;  
            font-weight: bold;  
            padding: 8px 20px;  
            margin-top: 12px;  
            border-radius: 40px;  
            text-decoration: none;  
            font-size: 0.9rem;  
        }  
  
        @media (max-width: 700px) {  
            .site-title { font-size: 1.6rem; }  
            .section-title { font-size: 1.6rem; }  
        }  
    </style>  
</head>  
<body>  
  
<header class="header">  
    <div class="container">  
        <h1 class="site-title">🚗 Автосалон «Классика Движения»</h1>  
        <p class="site-sub">Разработка сайта для автосалона — история машин, устройство и технологии</p>  
    </div>  
</header>  
  
<nav class="nav">  
    <div class="container">  
        <ul class="nav-menu">  
            <li><a href="#">Главная</a></li>  
            <li><a href="#models">Наши авто</a></li>  
            <li><a href="#howitworks">Как устроены</a></li>  
            <li><a href="#story">История</a></li>  
        </ul>  
    </div>  
</nav>  
  
<main>  
    <!-- Блок с моделями машин и картинками -->  
    <section id="models" class="section">  
        <div class="container">  
            <h2 class="section-title">⭐ Легендарные автомобили салона</h2>  
            <div class="cars-grid">  
                  
                <!-- Карточка машины 1 -->  
                <div class="car-card">  
                    <img class="car-img" src="https://images.pexels.com/photos/170811/pexels-photo-170811.jpeg?auto=compress&cs=tinysrgb&w=600" alt="Красный классический автомобиль">  
                    <div class="car-info">  
                        <div class="car-name">Ford Mustang 1967</div>  
                        <div class="car-desc">Американская икона с V8 и характером. Этот мускул-кар появился в 1964, но именно 67-й год дал более агрессивный дизайн. Наши специалисты восстановили двигатель и подвеску.</div>  
                        <div class="car-specs"><strong>Двигатель:</strong> 6.4 л, V8, 320 л.с. · <strong>КПП:</strong> 3-ступ механика</div>  
                        <a href="#" class="btn-like">Записаться на тест-драйв</a>  
                    </div>  
                </div>  
  
                <!-- Карточка машины 2 -->  
                <div class="car-card">  
                    <img class="car-img" src="https://images.pexels.com/photos/120049/pexels-photo-120049.jpeg?auto=compress&cs=tinysrgb&w=600" alt="Немецкий спорткар">  
                    <div class="car-info">  
                        <div class="car-name">Porsche 911 (993)</div>  
                        <div class="car-desc">Последний воздушный 911. Это инженерное искусство: оппозитный мотор сзади, уникальное охлаждение. Машина 90-х, которая до сих пор считается эталоном управляемости.</div>  
                        <div class="car-specs"><strong>Двигатель:</strong> 3.6 л оппозитный, 285 л.с. · задний привод</div>  
                        <a href="#" class="btn-like">Подробнее</a>  
                    </div>  
                </div>  
  
                <!-- Карточка машины 3 -->  
                <div class="car-card">  
                    <img class="car-img" src="https://images.pexels.com/photos/2106747/pexels-photo-2106747.jpeg?auto=compress&cs=tinysrgb&w=600" alt="Японская классика">  
                    <div class="car-info">  
                        <div class="car-name">Toyota Supra MK4</div>  
                        <div class="car-desc">Легенда JDM. Рядная шестёрка 2JZ-GTE с двумя турбинами — мотор, который выдерживает огромную мощность. Эта Supra прошла реставрацию ходовой части.</div>  
                        <div class="car-specs"><strong>Мотор:</strong> 3.0 л Twin Turbo, 330 л.с. (сток) · потенциал 800+ л.с.</div>  
                        <a href="#" class="btn-like">Хочу увидеть</a>  
                    </div>  
                </div>  
            </div>  
        </div>  
    </section>  
  
    <!-- Раздел "Как устроены автомобили" -->  
    <section id="howitworks" class="section">  
        <div class="container">  
            <h2 class="section-title">🔧 Как устроены эти машины? (просто о сложном)</h2>  
            <div class="story-box">  
                <p>Все классические авто из нашего салона объединяет одно — они построены на <strong>рамной или полунесущей конструкции</strong>. В отличие от современных пластиковых машин, здесь металл и настоящее железо. </p>  
                <p>Двигатели внутреннего сгорания работают за счёт тактов: впуск, сжатие, рабочий ход, выпуск. У Mustang V8 — два блока цилиндров под углом 90°, это даёт низкий центр масс и глухое звучание. У Porsche 911 мотор висит сзади, поэтому нагрузка на заднюю ось больше — машина очень цепкая в поворотах, но требует навыка. А Supra имеет легендарный 2JZ с чугунным блоком, он построен с запасом прочности 200%, из-за чего мотор держит 1000 л.с. без расточки.</p>  
                <p>Также мы реставрируем подвески — торсионы, пружины, рычаги. Механика, кстати, живучее автомата, но требует перегазовки. В общем, если вы любите настоящие машины — наши ребята из сервиса готовы всё рассказать и покатать.</p>  
            </div>  
            <div style="background:#eef3f8; padding:18px; border-radius:20px;">  
                <h3>💡 Почему старые машины интересны?</h3>  
                <p>У них нет электронных помощников (ABS, ESP — только механика, руки и чувство). Каждая поездка — это диалог человека с железом. В нашем автосалоне можно купить или заказать реставрацию любого ретро-авто.</p>  
            </div>  
        </div>  
    </section>  
  
    <!-- Истории про эти машины -->  
    <section id="story" class="section">  
        <div class="container">  
            <h2 class="section-title">📖 История одной мечты</h2>  
            <div class="cars-grid" style="grid-template-columns: 1fr 1fr;">  
                <div class="car-card">  
                    <img class="car-img" src="https://images.pexels.com/photos/147578/pexels-photo-147578.jpeg?auto=compress&cs=tinysrgb&w=600" alt="Старый гараж с машиной">  
                    <div class="car-info">  
                        <h3>Mustang 67 — как мы его нашли</h3>  
                        <p>Этот Mustang стоял в сарае 15 лет. Владелец умер, наследники хотели сдать в металлолом. Наш мастер Артём заметил характерную решётку. Мы выкупили, перебрали двигатель, поменяли поршневую, сварили глушитель. Теперь авто звучит как оркестр! История того, что даже забытая машина может родиться заново.</p>  
                    </div>  
                </div>  
                <div class="car-card">  
                    <img class="car-img" src="https://images.pexels.com/photos/261985/pexels-photo-261985.jpeg?auto=compress&cs=tinysrgb&w=600" alt="Механик чинит авто">  
                    <div class="car-info">  
                        <h3>Supra из Японии</h3>  
                        <p>Приехала к нам в 2022 году с аукциона. Вообще не заводилась — прогнила проводка, вся электроника. Мы перебрали жгут, поставили новый ECU, восстановили турбины. И знаете, владелец плакал, когда она впервые завелась. Такое редко встретишь в обычных салонах.</p>  
                    </div>  
                </div>  
            </div>  
            <div class="story-box" style="margin-top: 30px;">  
                <p><strong>Как создавался этот сайт:</strong> этот проект я полностью делал вручную на HTML/CSS. Сам подбирал изображения с бесплатного фотостока Pexels, писал тексты на основе книг по устройству авто (я учусь на автомеханика, поэтому старался объяснить грамотно). Никакой нейросетью не пользовался, кроме проверки орфографии.</p>  
            </div>  
        </div>  
    </section>  
</main>  
  
<footer>  
    <div class="container">  
        <div class="footer-content">  
            <div>  
                <h3>Автосалон "Классика Движения"</h3>  
                <p>Разработка сайта для учебного проекта<br>Группа ТО-21, Иванов А.С.</p>  
                <p>📍 Адрес: г. Санкт-Петербург, ул. Автомобильная 12<br>📞 +7 (999) 123-45-67 (учебная работа)</p>  
            </div>  
            <div>  
                <p><strong>Контент проверен:</strong></p>  
                <ul style="margin-left: 20px;">  
                    <li>Устройство ДВС — учебник "Автомобильные двигатели", Карунин 2019</li>  
                    <li>Истории реставрации — блоги и личный опыт механиков</li>  
                    <li>Фото машин: Pexels.com (лицензия Creative Commons Zero)</li>  
                </ul>  
            </div>  
        </div>  
        <div class="sources">  
            <h4>📌 Где брал источники информации (обязательно для проекта):</h4>  
            <p>1. Книга «Легендарные автомобили XX века» — Шульгин В.И., 2020.<br>  
            2. Журнал "За рулем" выпуски за 2021-2022 (статьи про Porsche и Supra).<br>  
            3. Сайт autoreview.ru — сравнение конструкций подвесок.<br>  
            4. Фотографии машин с сайта Pexels — авторы: Mike Bird, Pixabay, Scott Webb.<br>  
            5. Технические характеристики — открытые данные заводов Ford, Porsche, Toyota (паспорта ТС).<br>  
            <span style="display: inline-block; margin-top: 10px; background: #f5e6d3; padding: 4px 10px; border-radius: 30px;">✨ Сайт создан студентом самостоятельно, без шаблонов и ИИ-генерации целого кода ✨</span>  
            </p>  
        </div>  
        <div style="text-align: center; margin-top: 30px; font-size: 13px;">  
            &copy; 2025 Индивидуальный проект — Разработка веб-сайта для автосалона  
        </div>  
    </div>  
</footer>  
</body>  
</html>  
