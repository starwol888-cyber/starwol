<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Starwol - Sculptures en Pierre de Tuffeau</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        header {
            background-color: #333;
            color: white;
            padding: 10px 20px;
            text-align: center;
        }

        nav ul {
            list-style-type: none;
            padding: 0;
        }

        nav ul li {
            display: inline;
            margin-right: 15px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
        }

        section {
            padding: 20px;
            margin: 10px;
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        .product {
            border: 1px solid #ccc;
            padding: 10px;
            margin: 10px 0;
            text-align: center;
        }

        .product img {
            width: 100%;
            max-width: 200px;
        }

        footer {
            text-align: center;
            padding: 10px 0;
            background-color: #333;
            color: white;
        }

        form {
            display: flex;
            flex-direction: column;
        }

        form label {
            margin: 5px 0;
        }

        form input, form textarea {
            margin-bottom: 10px;
            padding: 8px;
            border-radius: 4px;
            border: 1px solid #ccc;
        }

        form button {
            padding: 10px;
            background-color: #333;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }

        form button:hover {
            background-color: #555;
        }
    </style>
</head>
<body>
    <header>
        <h1>Bienvenue chez Starwol</h1>
        <nav>
            <ul>
                <li><a href="#about">À propos</a></li>
                <li><a href="#products">Produits</a></li>
                <li><a href="#gallery">Galerie</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="about">
        <h2>À propos de nous</h2>
        <p>Starwol est dédié à la création de sculptures uniques en pierre de tuffeau, alliant tradition et innovation.</p>
    </section>

    <section id="products">
        <h2>Nos Sculptures</h2>
        <div class="product">
            <img src="images/sculpture1.jpg" alt="Sculpture 1">
            <h3>Sculpture 1</h3>
            <p>Prix : 200€</p>
            <button>Ajouter au panier</button>
        </div>
        <div class="product">
            <img src="images/sculpture2.jpg" alt="Sculpture 2">
            <h3>Sculpture 2</h3>
            <p>Prix : 250€</p>
            <button>Ajouter au panier</button>
        </div>
        <!-- Ajouter plus de sculptures ici -->
    </section>

    <section id="gallery">
        <h2>Galerie</h2>
        <p>Découvrez notre travail à travers ces photos et vidéos.</p>
        <img src="images/galerie1.jpg" alt="Galerie 1" style="width: 100%; max-width: 400px;">
        <img src="images/galerie2.jpg" alt="Galerie 2" style="width: 100%; max-width: 400px;">
        <!-- Ajouter des vidéos ici -->
    </section>

    <section id="contact">
        <h2>Contactez-nous</h2>
        <form>
            <label for="name">Nom :</label>
            <input type="text" id="name" name="name" required>
            <label for="email">Email :</label>
            <input type="email" id="email" name="email" required>
            <label for="message">Message :</label>
            <textarea id="message" name="message" required></textarea>
            <button type="submit">Envoyer</button>
        </form>
    </section>

    <footer>
        <p>© 2026 Starwol. Tous droits réservés.</p>
    </footer>

    <script>
        document.addEventListener("DOMContentLoaded", function() {
            const buttons = document.querySelectorAll('.product button');
            buttons.forEach(button => {
                button.addEventListener('click', () => {
                    alert('Produit ajouté au panier !');
                });
            });
        });
    </script>
</body>
</html>
