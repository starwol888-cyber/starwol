<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<title>Starwol – Site Officiel</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
:root {
    --dark: #0b2d33;
    --primary: #0f4c5c;
    --accent: #38b2ac;
    --light: #e6fffa;
}

* {
    box-sizing: border-box;
}

body {
    margin: 0;
    font-family: 'Segoe UI', Arial, sans-serif;
    background: linear-gradient(135deg, var(--dark), var(--primary));
    color: var(--light);
}

/* ===== HEADER ===== */
header {
    text-align: center;
    padding: 80px 20px;
    background: rgba(0,0,0,0.35);
}

header h1 {
    font-size: 3rem;
    letter-spacing: 4px;
    margin-bottom: 10px;
}

/* ===== SECTIONS ===== */
section {
    padding: 80px 20px;
    max-width: 1100px;
    margin: auto;
}

/* Animation scroll */
.reveal {
    opacity: 0;
    transform: translateY(40px);
    transition: all 0.8s ease;
}

.reveal.active {
    opacity: 1;
    transform: translateY(0);
}

h2 {
    text-align: center;
    font-size: 2.4rem;
    margin-bottom: 40px;
    color: var(--accent);
}

/* ===== GALERIE ===== */
.gallery {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 25px;
}

.gallery img {
    width: 100%;
    border-radius: 18px;
    cursor: pointer;
    transition: transform 0.4s, box-shadow 0.4s;
}

.gallery img:hover {
    transform: scale(1.06);
    box-shadow: 0 0 25px rgba(56,178,172,0.7);
}

/* ===== LIGHTBOX ===== */
.lightbox {
    position: fixed;
    inset: 0;
    background: rgba(0,0,0,0.9);
    display: none;
    align-items: center;
    justify-content: center;
    z-index: 1000;
}

.lightbox img {
    max-width: 90%;
    max-height: 90%;
    border-radius: 20px;
}

.lightbox.active {
    display: flex;
}

/* ===== FORMULAIRE ===== */
form {
    background: rgba(0,0,0,0.4);
    padding: 35px;
    border-radius: 25px;
    max-width: 500px;
    margin: auto;
    box-shadow: 0 0 30px rgba(0,0,0,0.6);
}

label {
    display: block;
    margin-top: 18px;
    font-weight: bold;
}

input, textarea {
    width: 100%;
    padding: 14px;
    margin-top: 8px;
    border-radius: 12px;
    border: none;
    outline: none;
}

button {
    margin-top: 30px;
    width: 100%;
    padding: 16px;
    border-radius: 40px;
    border: none;
    background: linear-gradient(45deg, var(--accent), #2dd4bf);
    font-size: 1.1rem;
    font-weight: bold;
    cursor: pointer;
    transition: transform 0.3s, box-shadow 0.3s;
}

button:hover {
    transform: translateY(-4px);
    box-shadow: 0 0 25px rgba(45,212,191,0.8);
}

/* ===== FOOTER ===== */
footer {
    text-align: center;
    padding: 30px;
    background: rgba(0,0,0,0.6);
    font-size: 0.9rem;
}
</style>
</head>

<body>

<header class="reveal">
    <h1>Starwol</h1>
    <p>Là où la créativité rencontre la puissance</p>
</header>

<main>

<section id="galerie" class="reveal">
    <h2>Galerie</h2>
    <div class="gallery">
        <img src="image1.jpg" alt="Galerie 1">
        <img src="image2.jpg" alt="Galerie 2">
        <img src="image3.jpg" alt="Galerie 3">
    </div>
</section>

<section id="contact" class="reveal">
    <h2>Contactez-nous</h2>
    <form action="#" method="post">
        <label for="name">Nom</label>
        <input type="text" id="name" required>

        <label for="email">Email</label>
        <input type="email" id="email" required>

        <label for="message">Message</label>
        <textarea id="message" rows="5" required></textarea>

        <button type="submit">Envoyer 🚀</button>
    </form>
</section>

</main>

<footer>
    <p>© 2026 Starwol. Tous droits réservés.</p>
</footer>

<!-- Lightbox -->
<div class="lightbox" id="lightbox">
    <img src="" alt="Image plein écran">
</div>

<script>
/* ===== SCROLL ANIMATION ===== */
const reveals = document.querySelectorAll(".reveal");

function revealOnScroll() {
    reveals.forEach(el => {
        const top = el.getBoundingClientRect().top;
        if (top < window.innerHeight - 100) {
            el.classList.add("active");
        }
    });
}
window.addEventListener("scroll", revealOnScroll);
revealOnScroll();

/* ===== GALERIE PLEIN ÉCRAN ===== */
const images = document.querySelectorAll(".gallery img");
const lightbox = document.getElementById("lightbox");
const lightboxImg = lightbox.querySelector("img");

images.forEach(img => {
    img.addEventListener("click", () => {
        lightboxImg.src = img.src;
        lightbox.classList.add("active");
    });
});

lightbox.addEventListener("click", () => {
    lightbox.classList.remove("active");
});
</script>

</body>
</html>
