<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Timval Secure - Votre Guide Ultime de Sécurité des Mots de Passe</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: #181818;
            color: #f0f0f0;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }
        header {
            background-color: #282828;
            padding: 20px;
            text-align: center;
            border-bottom: 1px solid #383838;
        }
        nav ul {
            list-style: none;
            padding: 0;
            margin: 15px 0;
            display: flex;
            justify-content: center;
        }
        nav a {
            color: #aaa;
            text-decoration: none;
            padding: 10px 20px;
            margin: 0 10px;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }
        nav a:hover {
            background-color: #383838;
            color: #eee;
        }
        main {
            flex-grow: 1;
            padding: 30px;
            display: grid;
            grid-template-columns: 1fr;
            gap: 30px;
        }
        .panel {
            background-color: #222;
            padding: 25px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.6);
        }
        .panel h2 {
            color: #bbb;
            margin-top: 0;
            margin-bottom: 15px;
            text-align: center;
        }
        #password-tester label {
            display: block;
            margin-bottom: 8px;
            color: #ccc;
        }
        #password-input {
            background-color: #333;
            color: #eee;
            padding: 10px;
            margin-bottom: 15px;
            border: 1px solid #555;
            border-radius: 5px;
            width: 100%;
            box-sizing: border-box;
        }
        #test-button {
            background-color: #00aaff;
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
        #test-button:hover {
            background-color: #0088cc;
        }
        #result {
            margin-top: 15px;
            color: #ddd;
            font-weight: bold;
            text-align: center;
        }
        .security-info h3 {
            color: #bbb;
            margin-top: 20px;
            margin-bottom: 10px;
        }
        .security-info ul {
            list-style: disc;
            padding-left: 20px;
            color: #ccc;
            line-height: 1.6;
        }
        .security-info li {
            margin-bottom: 8px;
        }
        footer {
            background-color: #282828;
            color: #777;
            text-align: left;
            padding: 15px 20px;
            border-top: 1px solid #383838;
            font-size: 0.8em;
            position: fixed;
            bottom: 0;
            left: 0;
            width: 100%;
            box-sizing: border-box;
        }
        /* Ajoutez ici d'autres styles futuristes pour l'esthétique */
    </style>
</head>
<body>
    <header>
        <h1>Timval Secure</h1>
        <nav>
            <ul>
                <li><a href="#tester">Testeur de Mot de Passe</a></li>
                <li><a href="#menaces">Comprendre les Menaces</a></li>
                <li><a href="#securiser">Sécurité à Domicile</a></li>
                <li><a href="#apropos">À Propos</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section id="tester" class="panel">
            <h2>Testez la Sécurité de Votre Mot de Passe (Côté Client)</h2>
            <p style="color: #ccc;">Entrez un mot de passe pour évaluer sa robustesse (analyse basée sur des critères communs, aucune donnée n'est envoyée).</p>
            <label for="password-input">Mot de passe :</label>
            <input type="password" id="password-input" placeholder="Votre mot de passe ici">
            <button id="test-button">Évaluer</button>
            <div id="result"></div>
        </section>

        <section id="menaces" class="panel security-info">
            <h2>Comment les Hackers Procèdent-ils ?</h2>
            <p style="color: #ccc;">Comprendre les méthodes d'attaque est la première étape pour se protéger.</p>
            <ul>
                <li>
                    <h3>Attaques par Force Brute :</h3>
                    <p>Essai systématique de toutes les combinaisons possibles de caractères. Très long pour les mots de passe complexes.</p>
                </li>
                <li>
                    <h3>Attaques par Dictionnaire :</h3>
                    <p>Utilisation de listes de mots courants et de phrases probables.</p>
                </li>
                <li>
                    <h3>Ingénierie Sociale (Phishing) :</h3>
                    <p>Manipulation psychologique pour inciter à révéler des informations sensibles.</p>
                </li>
                <li>
                    <h3>Logiciels Malveillants (Keyloggers, Spyware) :</h3>
                    <p>Programmes enregistrant les frappes de clavier ou surveillant l'activité de l'utilisateur.</p>
                </li>
                <li>
                    <h3>Violation de Bases de Données :</h3>
                    <p>Les mots de passe hachés stockés sur des serveurs peuvent être compromis en cas de faille de sécurité.</p>
                </li>
                <li>
                    <h3>Attaques par Mot de Passe Divulgué :</h3>
                    <p>Utilisation de listes de mots de passe ayant fuité lors de précédentes violations de données.</p>
                </li>
            </ul>
        </section>

        <section id="securiser" class="panel security-info">
            <h2>Comment Bien Sécuriser Votre Espace Numérique à Domicile ?</h2>
            <p style="color: #ccc;">Adoptez ces pratiques pour renforcer votre sécurité en ligne.</p>
            <ul>
                <li>
                    <h3>Mots de Passe Forts et Uniques :</h3>
                    <p>Utilisez des combinaisons complexes de lettres (majuscules et minuscules), de chiffres et de symboles. Ne réutilisez jamais le même mot de passe sur plusieurs sites.</p>
                </li>
                <li>
                    <h3>Authentification à Deux Facteurs (2FA) :</h3>
                    <p>Activez cette option partout où elle est disponible. Elle ajoute une couche de sécurité supplémentaire en demandant un code en plus de votre mot de passe.</p>
                </li>
                <li>
                    <h3>Mises à Jour Régulières :</h3>
                    <p>Maintenez vos systèmes d'exploitation, navigateurs et applications à jour pour corriger les failles de sécurité.</p>
                </li>
                <li>
                    <h3>Soyez Vigilant Face au Phishing :</h3>
                    <p>Méfiez-vous des emails, SMS ou appels suspects vous demandant des informations personnelles. Vérifiez toujours l'authenticité de la source.</p>
                </li>
                <li>
                    <h3>Utilisez un Gestionnaire de Mots de Passe :</h3>
                    <p>Ces outils sécurisent et mémorisent vos mots de passe complexes, vous n'avez besoin de vous souvenir que d'un seul mot de passe maître.</p>
                </li>
                <li>
                    <h3>Sécurisez Votre Réseau Wi-Fi :</h3>
                    <p>Utilisez un mot de passe fort pour votre Wi-Fi et activez le chiffrement WPA3 si votre routeur le supporte.</p>
                </li>
                <li>
                    <h3>Pare-feu et Antivirus :</h3>
                    <p>Assurez-vous d'avoir un pare-feu actif et un logiciel antivirus à jour sur vos appareils.</p>
                </li>
                <li>
                    <h3>Prudence sur les Réseaux Publics :</h3>
                    <p>Évitez de saisir des informations sensibles sur les réseaux Wi-Fi publics. Utilisez un VPN si nécessaire.</p>
                </li>
            </ul>
        </section>

        <section id="apropos" class="panel">
            <h2>À Propos de Timval Secure</h2>
            <p style="color: #ccc;">Ce site a été créé par Timval pour sensibiliser à l'importance de la sécurité des mots de passe et fournir des conseils pratiques pour se protéger contre les menaces en ligne.</p>
        </section>
    </main>

    <footer>
        Produced by Timval
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const passwordInput = document.getElementById('password-input');
            const testButton = document.getElementById('test-button');
            const resultDiv = document.getElementById('result');

            testButton.addEventListener('click', function() {
                const password = passwordInput.value;
                const strength = assessPasswordStrength(password);
                resultDiv.textContent = `Force du mot de passe : ${strength}`;
                updateResultStyle(strength);
            });

            function assessPasswordStrength(password) {
                if (password.length < 8) {
                    return 'Faible';
                }
                const hasUpperCase = /[A-Z]/.test(password);
                const hasLowerCase = /[a-z]/.test(password);
                const hasNumbers = /[0-9]/.test(password);
                const hasSymbols = /[^\w\s]/.test(password);

                let strengthScore = 0;
                if (hasUpperCase) strengthScore++;
                if (hasLowerCase) strengthScore++;
                if (hasNumbers) strengthScore++;
                if (hasSymbols) strengthScore++;
                strengthScore += Math.min(password.length / 4, 5); // Bonus pour la longueur

                if (strengthScore <= 4) return 'Faible';
                if (strengthScore <= 7) return 'Moyen';
                return 'Fort';
            }

            function updateResultStyle(strength) {
                resultDiv.className = ''; // Réinitialise les classes précédentes
                if (strength === 'Faible') {
                    resultDiv.classList.add('weak');
                } else if (strength === 'Moyen') {
                    resultDiv.classList.add('medium');
                } else {
                    resultDiv.classList.add('strong');
                }
            }
        });
    </script>

    <style>
        /* Styles spécifiques pour le résultat du test de mot de passe */
        #result.weak {
            color: #ff4d4d; /* Rouge */
        }
        #result.medium {
            color: #ffc107; /* Jaune */
        }
        #result.strong {
            color: #28a745; /* Vert */
        }
    </style>
</body>
</html>
