<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vignoble [Nom de l'entreprise]</title>
    <link rel="stylesheet" href="styles.css">
    <script defer src="script.js"></script>
</head>
<body>
    <header>
        <h1>Vignoble [Nom de l'entreprise]</h1>
        <nav>
            <ul>
                <li><a href="#accueil">Accueil</a></li>
                <li><a href="#produits">Produits</a></li>
                <li><a href="#a-propos">À propos</a></li>
                <li><a href="#contact">Contact</a></li>
                <li><a href="#panier">Panier</a></li>
            </ul>
        </nav>
    </header>

    <section id="accueil">
        <h2>Bienvenue sur notre site</h2>
        <p>Découvrez nos vins d'exception et notre savoir-faire unique.</p>
    </section>

    <section id="produits">
        <h2>Nos Produits</h2>
        <div class="produit">
            <h3>Jus de Raisin</h3>
            <p>Notre jus de raisin est 100% naturel, sans additifs.</p>
            <p>Prix : 5€</p>
            <button onclick="ajouterAuPanier('Jus de Raisin', 5)">Ajouter au panier</button>
        </div>
        <div class="produit">
            <h3>Vin</h3>
            <p>Un vin rouge raffiné, parfait pour vos repas.</p>
            <p>Prix : 15€</p>
            <button onclick="ajouterAuPanier('Vin', 15)">Ajouter au panier</button>
        </div>
        <div class="produit">
            <h3>Grand Cru</h3>
            <p>Un grand cru d'exception pour les amateurs de vin.</p>
            <p>Prix : 50€</p>
            <button onclick="ajouterAuPanier('Grand Cru', 50)">Ajouter au panier</button>
        </div>
    </section>

    <section id="panier">
        <h2>Panier</h2>
        <ul id="panier-items"></ul>
        <p>Total : <span id="total">0</span>€</p>
    </section>

    <section id="a-propos">
        <h2>À propos de nous</h2>
        <p>Nous sommes un vignoble familial situé au cœur de [région]. Nous produisons des vins de qualité depuis plusieurs générations.</p>
    </section>

    <section id="contact">
        <h2>Contactez-nous</h2>
        <form id="contact-form">
            <label for="nom">Nom:</label>
            <input type="text" id="nom" name="nom" required>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea>
            <button type="submit">Envoyer</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2024 Vignoble [Nom de l'entreprise]. Tous droits réservés.</p>
    </footer>
</body>
</html>
2. Styles CSS
Crée un fichier styles.css :

css
Copier le code
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

header {
    background-color: #333;
    color: white;
    padding: 10px 0;
    text-align: center;
}

nav ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-weight: bold;
}

section {
    padding: 20px;
    margin: 20px;
    background-color: white;
    border-radius: 8px;
}

section#produits {
    display: flex;
    justify-content: space-around;
}

.produit {
    border: 1px solid #ccc;
    padding: 10px;
    border-radius: 8px;
    width: 30%;
    text-align: center;
}

button {
    background-color: #333;
    color: white;
    padding: 10px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}

button:hover {
    background-color: #555;
}

footer {
    text-align: center;
    padding: 20px;
    background-color: #333;
    color: white;
}
