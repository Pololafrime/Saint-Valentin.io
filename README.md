<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jeu de Piste - Saint-Valentin</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #ffe6e6;
            color: #333;
            margin: 0;
            padding: 0;
            text-align: center;
        }
        header {
            background-color: #ff9999;
            padding: 20px;
        }
        header h1 {
            color: white;
            font-size: 2.5em;
        }
        .container {
            max-width: 800px;
            margin: 20px auto;
            padding: 20px;
            background: white;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            border-radius: 8px;
        }
        .button {
            display: inline-block;
            margin: 10px auto;
            padding: 10px 20px;
            background-color: #ff6666;
            color: white;
            text-decoration: none;
            font-weight: bold;
            border-radius: 5px;
        }
        .button:hover {
            background-color: #cc5050;
        }
        footer {
            margin-top: 20px;
            font-size: 0.8em;
            color: #777;
        }
    </style>
</head>
<body>
    <header>
        <h1>Jeu de Piste - Spécial Saint-Valentin</h1>
    </header>

    <div class="container">
        <h2>Bienvenue, mon amour ❤️</h2>
        <p>Prête à te lancer dans une aventure ? Ce jeu est rempli d’énigmes et de surprises, conçu spécialement pour toi. Chaque étape te rapprochera un peu plus d’un petit trésor caché…</p>
        <p><strong>Indice n°1 :</strong> Regarde attentivement cette page, parfois les réponses se cachent juste devant toi…</p>
        <p>Quand tu es prête, clique ci-dessous pour commencer :</p>
        <a href="etape1.md" class="button">Commencer l’aventure</a>
    </div>

    <footer>
        &copy; 2025 | Créé avec amour ❤️
    </footer>
</body>
</html>

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Page protégée</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f4f4f4;
        }
        .container {
            text-align: center;
            background: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
        input[type="password"] {
            padding: 10px;
            width: 200px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        button {
            padding: 10px 20px;
            background-color: #007BFF;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        button:hover {
            background-color: #0056b3;
        }
        .error {
            color: red;
            margin-top: 10px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>Entrez le mot de passe</h2>
        <form id="passwordForm">
            <input type="password" id="password" placeholder="Mot de passe" required>
            <br>
            <button type="submit">Entrer</button>
            <p id="errorMessage" class="error" style="display: none;">Mot de passe incorrect</p>
        </form>
    </div>

    <script>
        document.getElementById('passwordForm').addEventListener('submit', function(event) {
            event.preventDefault();
            const password = document.getElementById('password').value;
            const correctPassword = '12345'; // Remplacez par le mot de passe désiré

            if (password === correctPassword) {
                window.location.href = 'page-secrete.html'; // Redirige vers une page protégée
            } else {
                const errorMessage = document.getElementById('errorMessage');
                errorMessage.style.display = 'block';
            }
        });
    </script>
</body>
</html>
