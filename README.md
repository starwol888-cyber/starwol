<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<title>Starwol – Taille de Pierre de Tuffeau</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
/* ===== COULEURS PRINCIPALES ===== */
:root {
    --vert-canard: #0f4c5c;
    --bleu-clair: #38b2ac;
    --sable: #f4e7c5;
    --gris-fonce: #2a2a2a;
    --blanc: #ffffff;
    --ombre: rgba(0, 0, 0, 0.4);
}

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: 'Segoe UI', Arial, sans-serif;
    background-color: var(--sable);
    color: var(--gris-fonce);
}

header {
    background: var(--vert-canard);
    color: var(--blanc);
    text-align: center;
    padding: 80px 20px;
}

header h1 {
    font-size: 3.2rem;
    letter-spacing: 4px;
    font-weight: bold;
    margin-bottom: 10px;
}

header p {
    font-size: 1.2rem;
    font-style: italic;
}

/* ===== NAVIGATION ===== */
nav {
    background: var(--bleu-clair);
    display: flex;
    justify-content: center;
    gap: 30px;
    padding: 15px 0;
    font-weight: bold;
}

nav a {
    color: var(--blanc);
    text-decoration: none;
    font-size: 1rem;
    transition: all 0.3s ease;
}

nav a:hover {
    color: var(--gris-fonce);
}

/* ===== GALERIE + SHOP ===== */
section {
    padding: 60px 20px;
    max-width: 1200px;
    margin: auto;
}

h2 {
    text-align: center;
    margin-bottom: 30px;
    color: var(--vert-canard);
    font-size: 2.4rem;
}

.gallery {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(230px, 1fr));
    gap: 25px;
}

.card {
    background: var(--blanc);
    border-radius: 15px;
    box-shadow: 0 0 15px var(--ombre);
    overflow: hidden;
    transition: transform 0.3s;
}

.card:hover {
    transform: scale(1.05);
}

.card img {
    width: 100%;
}

.card-content {
    padding: 15px;
    text-align: center;
}

.card-content h3 {
    font-size: 1.3rem;
    margin-bottom: 8px;
    color: var(--vert-canard);
}

.card-content p {
    font-size: 1.1rem;
    color: var(--gris-fonce);
}

.price {
    font-size: 1.2rem;
    font-weight: bold;
    margin-top: 10px;
    color: var(--bleu-clair);
}

/* ===== AUTRES SECTIONS ===== */

section#about p,
section#contact p {
    font-size: 1.1rem;
    line-height: 1.6;
    margin-top: 10px;
}

form {
    background: var(--blanc);
    padding: 30px;
    border-radius: 20px;
    box-shadow: 0 0 20px var(--ombre);
}

input, textarea {
    width: 100%;
    margin-top: 8px;
    padding: 12px;
    border-radius: 8px;
    border: 1px solid var(--gris-fonce);
}

button {
    margin-top: 15px;
    width: 100%;
    padding: 14px;
    border: none;
    background: var(--vert-canard);
    color: var(--blanc);
    font-weight: bold;
    cursor: pointer;
    border-radius: 8px;
    transition: 0.3s;
}

button:hover {
    background: var(--bleu-clair);
}

/* ===== FOOTER ===== */
footer {
    text-align: center;
    padding: 25px;
    background: var(--gris-fonce);
    color: var(--blanc);
}

@media (max-width: 600px) {
    nav {
        flex-direction: column;
        gap: 15px;
    }
}
</style>
</head>

<body>

<header>
    <h1>Starwol</h1>
    <p>L’art de la pierre de tuffeau — Élégance & patrimoine</p>
</header>

<nav>
    <a href="#gallery">Galerie & Boutique</a>
    <a href="#about">À propos</a>
    <a href="#contact">Contact</a>
    <a href="#follow">Suivi Commande</a>
</nav>

<section id="gallery">
    <h2>Notre Galerie & Boutique</h2>
    <div class="gallery">
        <div class="card">
            <img src="piece1.jpg" alt="Pierre sculptée 1">
            <div class="card-content">
                <h3>Pierre Sculptée A</h3>
                <p>Œuvre façonnée à la main</p>
                <div class="price">€120</div>
            </div>
        </div>
        <div class="card">
            <img src="piece2.jpg" alt="Pierre sculptée 2">
            <div class="card-content">
                <h3>Pierre Sculptée B</h3>
                <p>Design architectural unique</p>
                <div class="price">€220</div>
            </div>
        </div>
        <div class="card">
            <img src="piece3.jpg" alt="Pierre sculptée 3">
            <div class="card-content">
                <h3>Pierre Sculptée C</h3>
                <p>Forme naturelle authentique</p>
                <div class="price">€180</div>
            </div>
        </div>
    </div>
</section>

<section id="about">
    <h2>À propos de Starwol</h2>
    <p>
        Starwol est une entreprise artisanale spécialisée dans la taille et la sculpture de pierre de tuffeau. 
        Inspirés par la richesse du patrimoine architectural et la lumière unique de cette pierre, nous créons des pièces d’exception,
        alliant tradition et design moderne. Chaque création raconte une histoire, façonnée avec passion et précision.
    </p>
</section>

<section id="contact">
    <h2>Contactez-nous</h2>
    <form>
        <label for="name">Nom complet</label>
        <input type="text" id="name" required>

        <label for="email">Email</label>
        <input type="email" id="email" required>

        <label for="message">Votre message</label>
        <textarea id="message" rows="5" required></textarea>

        <button type="submit">Envoyer</button>
    </form>
</section>

<section id="follow">
    <h2>Order Tracking (Suivi de Commande)</h2>
    <p>
        Pour suivre votre commande, entrez votre numéro de suivi ci-dessous.
    </p>
    <form>
        <label for="ordernum">Order Number</label>
        <input type="text" id="ordernum" required>
        <button type="submit">Track Order</button>
    </form>
</section>

<footer>
    <p>© 2026 Starwol. Tous droits réservés.</p>
</footer>

</body>
</html>
