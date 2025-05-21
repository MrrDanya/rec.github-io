<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MrrDanya | Креативный дизайнер на заказ</title>
    <style>
        :root {
            --primary: #2ecc71;
            --primary-dark: #27ae60;
            --primary-light: #58d68d;
            --text: #2c3e50;
            --bg: #f8f9fa;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        
        body {
            font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
            background-color: var(--bg);
            color: var(--text);
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        header {
            background: linear-gradient(135deg, var(--primary), var(--primary-dark));
            color: white;
            text-align: center;
            padding: 3rem 1rem;
            position: relative;
            overflow: hidden;
        }
        
        .container {
            max-width: 100%;
            padding: 0 1.5rem;
            margin: 0 auto;
        }
        
        h1 {
            font-size: clamp(2rem, 5vw, 3rem);
            margin-bottom: 0.5rem;
            animation: fadeIn 0.8s ease-out;
        }
        
        .tagline {
            font-size: clamp(1rem, 3vw, 1.5rem);
            opacity: 0.9;
            animation: fadeIn 1s ease-out 0.3s both;
            max-width: 800px;
            margin: 0 auto;
        }
        
        section {
            padding: 3rem 0;
        }
        
        h2 {
            color: var(--primary-dark);
            font-size: clamp(1.5rem, 4vw, 2rem);
            text-align: center;
            margin-bottom: 2rem;
            position: relative;
        }
        
        h2::after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background: var(--primary);
            margin: 0.5rem auto 0;
            border-radius: 2px;
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(min(300px, 100%), 1fr));
            gap: 1.5rem;
            margin: 2rem 0;
        }
        
        .service-card {
            background: white;
            border-radius: 12px;
            padding: 1.8rem;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: all 0.3s ease;
            border: 1px solid rgba(0,0,0,0.05);
        }
        
        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.1);
        }
        
        .service-card h3 {
            color: var(--primary-dark);
            font-size: 1.3rem;
            margin-bottom: 0.8rem;
            display: flex;
            align-items: center;
        }
        
        .service-card h3::before {
            content: '✓';
            color: var(--primary);
            margin-right: 0.5rem;
            font-weight: bold;
        }
        
        .cta-section {
            text-align: center;
            background: white;
            border-radius: 12px;
            padding: 3rem 2rem;
            margin: 3rem auto;
            max-width: 800px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.08);
            border: 1px solid rgba(0,0,0,0.05);
        }
        
        .tg-btn {
            display: inline-block;
            background: var(--primary);
            color: white;
            padding: 0.9rem 2rem;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            font-size: 1.1rem;
            margin-top: 1.5rem;
            transition: all 0.3s ease;
            box-shadow: 0 4px 12px rgba(46, 204, 113, 0.3);
            border: none;
            cursor: pointer;
        }
        
        .tg-btn:hover {
            background: var(--primary-dark);
            transform: translateY(-2px);
            box-shadow: 0 6px 18px rgba(46, 204, 113, 0.4);
        }
        
        .universal-list {
            max-width: 700px;
            margin: 0 auto;
        }
        
        .universal-list ul {
            columns: 2;
            list-style-type: none;
        }
        
        .universal-list li {
            margin-bottom: 0.8rem;
            position: relative;
            padding-left: 1.5rem;
            break-inside: avoid;
        }
        
        .universal-list li::before {
            content: '•';
            color: var(--primary);
            position: absolute;
            left: 0;
            font-size: 1.2rem;
        }
        
        footer {
            text-align: center;
            padding: 2rem;
            background: var(--text);
            color: white;
            margin-top: 3rem;
        }
        
        @media (max-width: 768px) {
            .container {
                padding: 0 1rem;
            }
            
            section {
                padding: 2rem 0;
            }
            
            .universal-list ul {
                columns: 1;
            }
            
            .service-card {
                padding: 1.5rem;
            }
            
            .cta-section {
                padding: 2rem 1rem;
                margin: 2rem 0;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>MrrDanya</h1>
            <p class="tagline">Профессиональный дизайн любой сложности под ваш запрос</p>
        </div>
    </header>
    
    <main class="container">
        <section>
            <h2>Мои услуги</h2>
            <div class="services-grid">
                <div class="service-card">
                    <h3>Персонализированные аватары</h3>
                    <p>Уникальные портреты и аватары в любом стиле: от минимализма до детализированных иллюстраций с учетом всех ваших пожеланий.</p>
                </div>
                
                <div class="service-card">
                    <h3>Дизайнерские QR-коды</h3>
                    <p>Стильные QR-коды с индивидуальным дизайном, которые гармонично впишутся в ваш брендинг и привлекут внимание.</p>
                </div>
                
                <div class="service-card">
                    <h3>Авторские стикеры</h3>
                    <p>Эксклюзивные стикерпаки для мессенджеров с вашими персонажами или в выбранной тематике.</p>
                </div>
                
                <div class="service-card">
                    <h3>Логотипы и брендинг</h3>
                    <p>Разработка запоминающихся логотипов и фирменного стиля для бизнеса или личного бренда.</p>
                </div>
                
                <div class="service-card">
                    <h3>Оформление соцсетей</h3>
                    <p>Полный дизайн-контент для Instagram, Telegram, VK и других платформ: шапки, посты, stories.</p>
                </div>
                
                <div class="service-card">
                    <h3>карточки</h3>
                    <p>красивые карточки для маркетплейсов как вб, озон и т.д..</p>
                </div>
            </div>
        </section>
        
        <section>
            <h2>Что еще я делаю</h2>
            <div class="universal-list">
                <ul>
                    <li>Дизайн презентаций</li>
                    <li>Оформление YouTube каналов</li>
                    <li>Баннеры и рекламные макеты</li>
                    <li>Дизайн интерфейсов</li>
                    <li>Векторная графика</li>
                    <li>3D-моделирование</li>
                    <li>Персонажи для игр</li>
                    <li>Кастомные шрифты</li>
                </ul>
            </div>
        </section>
        
        <section class="cta-section">
            <h2>Готов реализовать ваш проект!</h2>
            <p>Делаю качественно, быстро и с индивидуальным подходом. Работаю до полного вашего удовлетворения результатом.</p>
            <a href="https://t.me/MrrDanya" class="tg-btn">Заказать в Telegram @MrrDanya</a>
            <p style="margin-top: 1rem; font-size: 0.9rem; opacity: 0.8;">Отвечаю в течение 15 минут в рабочее время</p>
        </section>
    </main>
    
    <footer>
        <div class="container">
            <p>© 2024 MrrDanya Creative Studio. Все права защищены.</p>
        </div>
    </footer>
</body>
</html>