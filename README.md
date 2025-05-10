<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Quvanchbekning Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <nav>
        <ul>
            <li><a href="#home">Bosh Sahifa</a></li>
            <li><a href="#about">Men Haqimda</a></li>
            <li><a href="#services">Xizmatlar</a></li>
            <li><a href="#contact">Aloqa</a></li>
        </ul>
    </nav>

    <section id="home" class="fade-in">
        <div class="hero">
            <h1>Salom, Men Quvanchbek!</h1>
            <p>Freelance veb-dasturchi | Animatsiyali va chiroyli saytlar yarataman</p>
            <a href="#contact" class="btn">Menga Yozing</a>
        </div>
    </section>

    <section id="about" class="fade-in">
        <h2>Men Haqimda</h2>
        <p>Men Quvanchbek, 21 yoshdaman. Veb-dasturlashni o‘rganayotgan ijodkorman. Mijozlarimga zamonaviy va sifatli xizmat ko‘rsataman.</p>
    </section>

    <section id="services" class="fade-in">
        <h2>Xizmatlarim</h2>
        <div class="services-container">
            <div class="service-box">
                <h3>Portfolio Saytlari</h3>
                <p>Shaxsiy yoki biznes uchun zamonaviy saytlar.</p>
            </div>
            <div class="service-box">
                <h3>Animatsiyali Dizayn</h3>
                <p>Chiroyli animatsiyalar bilan saytlar yarataman.</p>
            </div>
            <div class="service-box">
                <h3>Landing Page</h3>
                <p>Mahsulot yoki xizmat uchun landing page.</p>
            </div>
        </div>
    </section>

    <section id="contact" class="fade-in">
        <h2>Aloqa</h2>
        <p>Telegram: <a href="https://t.me/juniorQUVANCHBEK">@juniorQUVANCHBEK</a></p>
        <p>Email: <a href="mailto:quvanchbek79@gmail.com">quvanchbek79@gmail.com</a></p>
        <form>
            <input type="text" placeholder="Ismingiz" required>
            <input type="email" placeholder="Emailingiz" required>
            <textarea placeholder="Xabaringiz" required></textarea>
            <button type="submit" class="btn">Yuborish</button>
        </form>
    </section>

    <footer>
        <p>© 2025 Quvanchbek. Barcha huquqlar himoyalangan.</p>
    </footer>
</body>
</html>* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    background: #e8f5e9; /* O‘zgartirilgan orqa fon rangi - och yashil */
    line-height: 1.6;
}

nav {
    background-color: #2c3e50;
    padding: 15px 0;
    position: sticky;
    top: 0;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

nav ul {
    list-style: none;
    display: flex;
    justify-content: center;
}

nav ul li {
    margin: 0 20px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-weight: bold;
    transition: color 0.3s;
}

nav ul li a:hover {
    color: #e74c3c;
}

section {
    padding: 60px 20px;
    text-align: center;
}

.fade-in {
    opacity: 0;
    transform: translateY(20px);
    animation: fadeIn 1s forwards;
}

@keyframes fadeIn {
    to { opacity: 1; transform: translateY(0); }
}

#home {
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background: url('fon.jpg') no-repeat center/cover;
    color: white;
    text-shadow: 1px 1px 5px #000;
}

.hero h1 {
    font-size: 48px;
    margin-bottom: 10px;
}

.hero p {
    font-size: 20px;
    margin-bottom: 20px;
}

.btn {
    display: inline-block;
    padding: 12px 25px;
    background-color: #e74c3c;
    color: white;
    text-decoration: none;
    border-radius: 5px;
    transition: transform 0.3s, background-color 0.3s;
}

.btn:hover {
    background-color: #c0392b;
    transform: scale(1.1);
}

.services-container {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
}

.service-box {
    background-color: #fff;
    border: 1px solid #ddd;
    padding: 20px;
    width: 300px;
    border-radius: 10px;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s;
}

.service-box:hover {
    transform: translateY(-10px);
}

#contact form {
    max-width: 500px;
    margin: 0 auto;
}

#contact input, #contact textarea {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border: 1px solid #ddd;
    border-radius: 5px;
}

#contact button {
    background-color: #2c3e50;
    border: none;
    cursor: pointer;
}

#contact button:hover {
    background-color: #34495e;
}

footer {
    background-color: #2c3e50;
    color: white;
    text-align: center;
    padding: 20px;
    position: relative;
    bottom: 0;
    width: 100%;
}
