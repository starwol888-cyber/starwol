<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<title>Starwol – Taille de Pierre de Tuffeau</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
/* ===== PALETTE DE COULEURS (inspirée du style visuel) ===== */
:root {
    --bleu-principal: #3B82F6;
    --sable-clair: #F8F4E3;
    --vert-kaki: #6B8E23;
    --noir-profond: #1F1F1F;
    --orange-accent: #F59E0B;
    --gris-fonce: #333333;
    --blanc: #ffffff;
}

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: 'Segoe UI', Arial, sans-serif;
    background-color: var(--sable-clair);
    color: var(--gris-fonce);
}

/* ===== HEADER ===== */
header {
    background: var(--bleu-principal);
    color: var(--blanc);
    text-align: center;
    padding: 80px 20px;
}

header h1 {
    font-size: 3rem;
    letter-spacing: 4px;
    font-weight: bold;
    margin-bottom: 8px;
}

header p {
    font-size: 1.2rem;
    font-style: italic;
}

/* ===== NAVIGATION ===== */
nav {
    background: var(--noir-profond);
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
    transition: 0.3s;
}

nav a:hover {
    color: var(--orange-accent);
}

/* ===== SECTIONS ===== */
section {
    padding: 60px 20px;
    max-width: 1200px;
    margin: auto;
}

h2 {
    text-align: center;
    margin-bottom: 25px;
    color: var(--vert-kaki);
    font-size: 2.4rem;
}

/* ===== GALERIE & BOUTIQUE ===== */
.gallery {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    gap: 25px;
}

.card {
    background: var(--blanc);
    border-radius: 15px;
    box-shadow: 0px 0px 12px rgba(0,0,0,0.15);
    overflow: hidden;
    transition: transform 0.3s;
}

.card:hover {
    transform: scale(1.03);
}

.card img {
    width: 100%;
}

.card-content {
    padding: 15px;
    text-align: center;
}

.card-content h3 {
    font-size: 1.4rem;
    margin-bottom: 6px;
    color: var(--bleu-principal);
}

.card-content p {
    font-size: 1.1rem;
    color: var(--gris-fonce);
}

.price {
    font-size: 1.2rem;
    font-weight: bold;
    margin-top: 10px;
    color: var(--orange-accent);
}

/* ===== FORMULAIRE ===== */
form {
    background: var(--blanc);
    padding: 30px;
    border-radius: 20px;
    box-shadow: 0px 0px 20px rgba(0,0,0,0.1);
}

input, textarea {
    width: 100%;
    margin-top: 10px;
    padding: 12px;
    border-radius: 8px;
    border: 1px solid var(--gris-fonce);
}

button {
    margin-top: 18px;
    width: 100%;
    padding: 14px;
    border: none;
    background: var(--bleu-principal);
    color: var(--blanc);
    font-weight: bold;
    cursor: pointer;
    border-radius: 8px;
    transition: 0.3s;
}

button:hover {
    background: var(--orange-accent);
}

/* ===== FOOTER ===== */
footer {
    text-align: center;
    padding: 25px;
    background: var(--noir-profond);
    color: var(--blanc);
}
</style>
</head>

<body>

<header>
    <h1>Starwol</h1>
    <p>L’art de la taille de pierre de tuffeau & patrimoine vivant</p>
</header>

<nav>
    <a href="#gallery">Galerie & Boutique</a>
    <a href="#about">Biographie</a>
    <a href="#contact">Contact</a>
    <a href="#follow">Suivi Commande</a>
</nav>

<section id="gallery">
    <h2>Galerie & Boutique</h2>
    <div class="gallery">
        <div class="card">
            <img src="tuffeau1.jpg" alt="Pièce Sculptée A">
            <div class="card-content">
                <h3>Pièce Sculptée A</h3>
                <p>Pierre de tuffeau façonnée à la main</p>
                <div class="price">€150</div>
            </div>
        </div>
        <div class="card">
            <img src="tuffeau2.jpg" alt="Pièce Sculptée B">
            <div class="card-content">
                <h3>Pièce Sculptée B</h3>
                <p>Ouvrage décoratif pour architecture</p>
                <div class="price">€280</div>
            </div>
        </div>
        <div class="card">
            <img src="tuffeau3.jpg" alt="Pièce Sculptée C">
            <div class="card-content">
                <h3>Pièce Sculptée C</h3>
                <p>Design naturel et authentique</p>
                <div class="price">€200</div>
            </div>
        </div>
    </div>
</section>

<section id="about">
    <h2>Biographie de l'entreprise</h2>
    <p>
        Starwol est une entreprise artisanale spécialisée dans la taille de pierre de tuffeau, un
        matériau noble & emblématique du patrimoine. Fondée par des passionnés, notre mission est
        de créer des pièces uniques qui racontent une histoire — entre tradition et modernité,
        chaque création incarne la beauté brute du tuffeau et le savoir-faire français.
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
        <textarea id="message" rows="4" required></textarea>

        <button type="submit">Envoyer</button>
    </form>
</section>

<section id="follow">
    <h2>Order Tracking (Suivi de commande)</h2>
    <p>Enter your order number to track it:</p>
    <form>
        <input type="text" placeholder="Order Number" required>
        <button type="submit">Track Order</button>
    </form>
</section>

<footer>
    <p>© 2026 Starwol. Tous droits réservés.</p>
</footer>

</body>
</html>
