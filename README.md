<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TIMVAL SECURE : Votre Forteresse Numérique</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&family=Montserrat:wght@300;400;700&display=swap');

        /* Variables CSS pour un contrôle facile des couleurs */
        :root {
            --main-bg: #1a1a2e; /* Arrière-plan principal foncé */
            --secondary-bg: #16213e; /* Arrière-plan des sections/blocs */
            --accent-color: #0f3460; /* Couleur d'accentuation, pour la navigation par exemple */
            --text-color: #e0e0e0; /* Couleur du texte clair */
            --highlight-color: #e94560; /* Rouge futuriste pour les titres et accents */
            --border-color: #2e4a6e; /* Couleur des bordures et séparateurs */
            --button-hover: #cf3753; /* Couleur de survol pour les boutons */
        }

        body {
            font-family: 'Montserrat', sans-serif;
            margin: 0;
            padding: 0;
            background-color: var(--main-bg);
            color: var(--text-color);
            line-height: 1.7;
            overflow-x: hidden; /* Empêche le défilement horizontal indésirable */
        }

        /* Effet de fond subtil pour un look futuriste */
        body::before {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(circle at top left, rgba(233, 69, 96, 0.05) 0%, transparent 30%),
                        radial-gradient(circle at bottom right, rgba(15, 52, 96, 0.08) 0%, transparent 30%);
            z-index: -1;
        }

        header {
            background-color: var(--secondary-bg);
            padding: 40px 0;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
            border-bottom: 2px solid var(--highlight-color);
            position: relative;
            overflow: hidden;
        }

        header h1 {
            margin: 0;
            font-family: 'Orbitron', sans-serif;
            font-size: 3.2em;
            color: var(--highlight-color);
            text-shadow: 0 0 15px rgba(233, 69, 96, 0.6); /* Effet lumineux */
            letter-spacing: 2px;
        }

        header p {
            font-size: 1.1em;
            color: var(--text-color);
            margin-top: 10px;
        }

        /* Animation des particules en arrière-plan du header */
        header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: radial-gradient(circle, rgba(255,255,255,0.08) 1px, transparent 1px);
            background-size: 25px 25px;
            animation: move-bg 60s linear infinite;
        }

        @keyframes move-bg {
            from { background-position: 0 0; }
            to { background-position: 1000px 1000px; }
        }

        nav {
            background-color: var(--accent-color);
            padding: 15px 0;
            text-align: center;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.2);
            position: sticky; /* Rends la navigation collante lors du défilement */
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid var(--highlight-color);
        }

        nav a {
            color: var(--text-color);
            text-decoration: none;
            padding: 12px 25px;
            margin: 0 8px;
            border-radius: 5px;
            transition: background-color 0.3s ease, color 0.3s ease, transform 0.2s ease;
            font-weight: 700;
            font-family: 'Orbitron', sans-serif;
            font-size: 0.95em;
            display: inline-block;
            position: relative;
        }

        /* Effet de soulignement animé pour la navigation */
        nav a::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: 5px;
            left: 50%;
            background-color: var(--highlight-color);
            transition: width 0.3s ease, left 0.3s ease;
        }

        nav a:hover::after {
            width: calc(100% - 20px);
            left: 10px;
        }

        nav a:hover {
            background-color: rgba(233, 69, 96, 0.2);
            color: var(--highlight-color);
            transform: translateY(-2px);
        }

        .container {
            max-width: 1000px;
            margin: 30px auto;
            padding: 20px;
            background-color: var(--secondary-bg);
            border-radius: 10px;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.4);
            border: 1px solid var(--border-color);
        }

        section {
            margin-bottom: 40px;
            padding: 25px;
            border-bottom: 1px dashed var(--border-color); /* Ligne de séparation épurée */
        }

        section:last-of-type {
            border-bottom: none;
        }

        h2 {
            font-family: 'Orbitron', sans-serif;
            color: var(--highlight-color);
            font-size: 2.2em;
            margin-bottom: 20px;
            border-left: 4px solid var(--highlight-color);
            padding-left: 15px;
            text-shadow: 0 0 8px rgba(233, 69, 96, 0.4);
        }

        h3 {
            font-family: 'Montserrat', sans-serif;
            color: var(--text-color);
            font-size: 1.6em;
            margin-top: 30px;
            margin-bottom: 15px;
            border-bottom: 1px solid var(--border-color);
            padding-bottom: 5px;
        }

        p {
            margin-bottom: 15px;
        }

        ul {
            list-style-type: none; /* Supprime les puces par défaut */
            margin-left: 0;
            padding-left: 20px;
            margin-bottom: 15px;
        }

        ul li::before {
            content: "\2022"; /* Utilise une puce unicode */
            color: var(--highlight-color);
            font-weight: bold;
            display: inline-block;
            width: 1em;
            margin-left: -1em;
        }

        ol {
            list-style-type: decimal;
            margin-left: 20px;
            margin-bottom: 15px;
        }

        .password-tester {
            background-color: var(--accent-color);
            padding: 30px;
            border-radius: 8px;
            margin-top: 25px;
            text-align: center;
            box-shadow: inset 0 0 10px rgba(0, 0, 0, 0.3);
            border: 1px solid var(--highlight-color);
        }

        .password-tester label {
            display: block;
            margin-bottom: 15px;
            font-size: 1.2em;
            color: var(--highlight-color);
            font-family: 'Orbitron', sans-serif;
        }

        .password-tester input[type="password"] {
            width: calc(100% - 40px);
            padding: 15px;
            margin-bottom: 20px;
            border: 1px solid var(--border-color);
            border-radius: 5px;
            font-size: 1.1em;
            background-color: var(--main-bg);
            color: var(--text-color);
            max-width: 450px;
            transition: border-color 0.3s ease, box-shadow 0.3s ease;
        }

        .password-tester input[type="password"]:focus {
            outline: none;
            border-color: var(--highlight-color);
            box-shadow: 0 0 10px rgba(233, 69, 96, 0.5);
        }

        .password-strength {
            font-weight: bold;
            font-size: 1.2em;
            margin-top: 15px;
            padding: 12px;
            border-radius: 5px;
            transition: background-color 0.5s ease, color 0.5s ease;
        }

        /* Couleurs de force du mot de passe */
        .strength-0 { background-color: #a00000; color: white; } /* Très faible */
        .strength-1 { background-color: #d17a00; color: white; } /* Faible */
        .strength-2 { background-color: #d1b100; color: #333; } /* Moyenne */
        .strength-3 { background-color: #0a8d00; color: white; } /* Forte */
        .strength-4 { background-color: #006400; color: white; } /* Très forte */

        .icon {
            margin-right: 10px;
            color: var(--highlight-color);
            font-size: 1.1em;
        }

        footer {
            background-color: var(--accent-color);
            color: var(--text-color);
            text-align: center;
            padding: 25px 0;
            margin-top: 40px;
            box-shadow: 0 -4px 12px rgba(0, 0, 0, 0.2);
            border-top: 1px solid var(--highlight-color);
            font-size: 0.9em;
        }
    </style>
</head>
<body>
    <header>
        <h1><i class="fas fa-shield-alt"></i> TIMVAL SECURE</h1>
        <p>Votre Forteresse Numérique : Sécurisez votre Vie Privée et vos Données</p>
    </header>

    <nav>
        <a href="#trackers"><i class="fas fa-fingerprint"></i> Traqueurs</a>
        <a href="#hackers"><i class="fas fa-skull-crossbones"></i> Cyberattaques</a>
        <a href="#passwords"><i class="fas fa-key"></i> Mots de Passe</a>
        <a href="#tester"><i class="fas fa-terminal"></i> Testeur MP</a>
        <a href="#tips"><i class="fas fa-lightbulb"></i> Cyber-Astuces</a>
    </nav>

    <div class="container">
        <section id="trackers">
            <h2><i class="fas fa-fingerprint icon"></i> L'Ombre des Traqueurs en Ligne</h2>
            <p>Dans l'écosystème numérique actuel, les **traqueurs** sont omniprésents. Ces technologies invisibles (cookies, pixels, scripts) collectent silencieusement vos données de navigation. Bien qu'elles puissent améliorer l'expérience utilisateur ou personnaliser les publicités, leur collecte massive pose de sérieuses questions éthiques et de confidentialité.</p>

            <h3>Mécanismes de Traque :</h3>
            <ul>
                <li><strong>Cookies Tiers :</strong> Des fichiers déposés par des domaines autres que celui du site visité, permettant un suivi trans-sites de votre activité.</li>
                <li><strong>Pixels de Suivi :</strong> Petites images invisibles intégrées pour collecter des données sur votre interaction avec une page ou un e-mail.</li>
                <li><strong>Empreinte Numérique (Fingerprinting) :</strong> Une méthode avancée qui identifie votre appareil de manière unique via ses caractéristiques (navigateur, polices, configuration matérielle), même sans cookies.</li>
                <li><strong>Scripts de Suivi :</strong> Des fragments de code qui enregistrent vos actions sur un site web : clics, défilement, temps passé.</li>
            </ul>

            <h3>Les Risques de la Surveillance :</h3>
            <ul>
                <li><strong>Profilage Détaillé :</strong> La construction de profils comportementaux précis, incluant vos intérêts, habitudes et préférences.</li>
                <li><strong>Publicité Ciblée Intensive :</strong> Des publicités qui vous suivent agressivement sur diverses plateformes.</li>
                <li><strong>Violation de la Vie Privée :</strong> Votre activité en ligne est constamment surveillée et analysée, sans votre consentement éclairé.</li>
                <li><strong>Vulnérabilités :</strong> Les bases de données de traqueurs peuvent devenir des cibles pour les fuites de données.</li>
            </ul>

            <h3>Contre-Mesures Essentielles :</h3>
            <ul>
                <li>Optez pour des navigateurs axés sur la confidentialité (ex: **Brave**, **Firefox** avec protection renforcée).</li>
                <li>Installez des extensions de blocage de publicité et de traqueurs (ex: **uBlock Origin**, **Privacy Badger**).</li>
                <li>Configurez méticuleusement les paramètres de confidentialité de vos navigateurs et de tous vos comptes en ligne.</li>
                <li>Utilisez un **VPN** (Virtual Private Network) pour masquer votre adresse IP et chiffrer votre connexion, rendant le suivi plus difficile.</li>
            </ul>
        </section>

        ---

        <section id="hackers">
            <h2><i class="fas fa-skull-crossbones icon"></i> Les Menaces des Cyberattaques</h2>
            <p>Les **hackers** et les **cyberattaques** représentent une menace constante dans le paysage numérique. Leurs motivations sont diverses : vol de données, fraude financière, espionnage, sabotage, ou même simple démonstration de force. Les tactiques évoluent, rendant la vigilance plus cruciale que jamais.</p>

            <h3>Typologies d'Attaques Courantes :</h3>
            <ul>
                <li><strong>Phishing (Hameçonnage) :</strong> Des tentatives frauduleuses pour obtenir vos informations sensibles (mots de passe, numéros de carte bancaire) en se faisant passer pour une entité légitime (banque, service public, entreprise connue).</li>
                <li><strong>Malware (Logiciels Malveillants) :</strong> Vaste catégorie de logiciels conçus pour nuire ou accéder à des systèmes sans autorisation. Inclut :
                    <ul>
                        <li>**Virus :** Se répliquent et s'attachent à d'autres programmes.</li>
                        <li>**Ransomware (Rançongiciel) :** Chiffre vos données et exige une rançon pour leur déblocage.</li>
                        <li>**Spyware (Logiciel Espion) :** Collecte des informations à votre insu.</li>
                        <li>**Chevaux de Troie :** Se déguisent en programmes utiles pour infiltrer votre système.</li>
                    </ul>
                </li>
                <li><strong>Attaques DDoS (Déni de Service Distribué) :</strong> Saturent les serveurs avec un trafic massif, rendant les services en ligne indisponibles.</li>
                <li><strong>Attaques par Force Brute :</strong> Tentatives systématiques de deviner vos mots de passe en essayant toutes les combinaisons possibles.</li>
                <li><strong>Ingénierie Sociale :</strong> Exploitation de la psychologie humaine pour manipuler des individus afin qu'ils divulguent des informations confidentielles ou effectuent des actions non souhaitées.</li>
            </ul>

            <h3>Impacts d'une Compromission :</h3>
            <ul>
                <li>**Vol d'Identité :** Utilisation de vos informations personnelles à des fins frauduleuses.</li>
                <li>**Pertes Financières :** Fraude bancaire, rançons, accès non autorisé à vos comptes.</li>
                <li>**Atteinte à la Réputation :** Pour les individus et les entreprises.</li>
                <li>**Perte d'Accès :** Vos comptes ou vos systèmes peuvent être rendus inaccessibles.</li>
                <li>**Corruption de Données :** Altération ou destruction de vos fichiers importants.</li>
            </ul>
        </section>

        ---

        <section id="passwords">
            <h2><i class="fas fa-key icon"></i> L'Art du Mot de Passe Imprenable</h2>
            <p>Votre **mot de passe** est la première ligne de défense de votre identité numérique. Un mot de passe faible est une vulnérabilité majeure que les attaquants exploitent en priorité.</p>

            <h3>Les Axiomes d'un Mot de Passe Cyber-Robuste :</h3>
            <ol>
                <li><strong>La Longueur est Reine :</strong> Visez au moins **12 caractères**, idéalement 16 ou plus. La complexité augmente exponentiellement avec la longueur.</li>
                <li><strong>Diversité de Caractères :</strong> Intégrez un mélange de :
                    <ul>
                        <li>Lettres minuscules (a-z)</li>
                        <li>Lettres majuscules (A-Z)</li>
                        <li>Chiffres (0-9)</li>
                        <li>Caractères spéciaux (!@#$%^&*()_+-=[]{}|;':",.<>/?`~)</li>
                    </ul>
                </li>
                <li><strong>Unicité Absolue :</strong> Ne réutilisez **JAMAIS** le même mot de passe pour plusieurs comptes. Si une base de données est compromise, tous vos comptes associés sont en danger.</li>
                <li><strong>L'Évitement des Évidences :</strong> Bannissez les informations personnelles, les mots du dictionnaire, les séquences (123456) ou les claviers (azerty).</li>
                <li><strong>Phrases de Passe :</strong> Préférez des "phrases de passe" (passphrases) longues et mémorables plutôt que des mots complexes. Ex: "LeG4rd1enDuCyb3rEspac3!"</li>
                <li><strong>Authentification à Deux Facteurs (2FA/MFA) :</strong> Activez-la partout où c'est possible. Cela ajoute une couche de sécurité cruciale (code via SMS, application d'authentification, clé de sécurité).</li>
                <li><strong>Gestionnaires de Mots de Passe :</strong> Utilisez un logiciel fiable (**Bitwarden**, **LastPass**, **KeePass**) pour générer, stocker et remplir automatiquement vos mots de passe complexes. Vous n'aurez qu'un seul mot de passe maître à mémoriser.</li>
            </ol>
        </section>

        ---

        <section id="tester">
            <h2><i class="fas fa-terminal icon"></i> Analyseur de Force de Mot de Passe</h2>
            <p>Vérifiez la robustesse d'un mot de passe en temps réel. **N'utilisez PAS un de vos vrais mots de passe ici.** Cet outil est à des fins de démonstration uniquement.</p>
            <div class="password-tester">
                <label for="passwordInput">Entrez votre mot de passe à évaluer :</label>
                <input type="password" id="passwordInput" placeholder="Saisissez un mot de passe non réel...">
                <div id="passwordStrength" class="password-strength"></div>
            </div>
        </section>

        ---

        <section id="tips">
            <h2><i class="fas fa-lightbulb icon"></i> Cyber-Astuces Essentielles</h2>
            <ul>
                <li><strong>Mises à Jour Systématiques :</strong> Maintenez à jour votre système d'exploitation, vos navigateurs et toutes vos applications. Les mises à jour corrigent souvent des failles de sécurité critiques.</li>
                <li><strong>Antivirus & Anti-Malware :</strong> Utilisez une suite de sécurité réputée et assurez-vous qu'elle est toujours active et à jour.</li>
                <li><strong>Sauvegardes Régulières :</strong> Sauvegardez vos données importantes sur des supports externes ou des services cloud sécurisés. C'est votre filet de sécurité contre la perte de données.</li>
                <li><strong>Méfiance Digitale :</strong> Soyez extrêmement prudent avec les e-mails, les messages ou les appels inattendus, surtout s'ils demandent des informations personnelles ou financières. Vérifiez toujours la source.</li>
                <li><strong>Prudence sur le Wi-Fi Public :</strong> Évitez les transactions sensibles (banque, achats) sur des réseaux Wi-Fi publics non sécurisés. Un VPN est fortement recommandé dans ces situations.</li>
                <li><strong>Éducation Continue :</strong> La cybersécurité évolue. Restez informé des dernières menaces et bonnes pratiques.</li>
            </ul>
        </section>
    </div>

    <footer>
        <p>Ce site a été créé par la **timval** pour vous prévenir des dangers d'Internet et renforcer votre sécurité numérique.</p>
        <p>&copy; 2025 Timval Secure. Tous droits réservés. | Pour des conseils de sécurité personnalisés, consultez un expert.</p>
    </footer>

    <script>
        document.getElementById('passwordInput').addEventListener('input', function() {
            const password = this.value;
            const strengthDisplay = document.getElementById('passwordStrength');
            let strength = 0;
            let feedback = '';

            // Critères d'évaluation
            const hasLowercase = /[a-z]/.test(password);
            const hasUppercase = /[A-Z]/.test(password);
            const hasDigit = /[0-9]/.test(password);
            const hasSpecial = /[!@#$%^&*()_+\-=\[\]{};':"\\|,.<>\/?`~]/.test(password);

            // Points basés sur la longueur
            if (password.length >= 8) strength += 1;
            if (password.length >= 12) strength += 1;
            if (password.length >= 16) strength += 1;

            // Points basés sur la diversité des caractères
            if (hasLowercase) strength += 1;
            if (hasUppercase) strength += 1;
            if (hasDigit) strength += 1;
            if (hasSpecial) strength += 1;

            // Évaluation finale
            let strengthText = '';
            let strengthClass = '';

            if (password.length === 0) {
                strengthText = 'Veuillez entrer un mot de passe.';
                strengthClass = '';
            } else if (strength < 3) {
                strengthText = 'Très Faible';
                strengthClass = 'strength-0';
            } else if (strength >= 3 && strength < 5) {
                strengthText = 'Faible';
                strengthClass = 'strength-1';
            } else if (strength >= 5 && strength < 7) {
                strengthText = 'Moyenne';
                strengthClass = 'strength-2';
            } else if (strength >= 7 && strength < 9) {
                strengthText = 'Forte';
                strengthClass = 'strength-3';
            } else if (strength >= 9) {
                strengthText = 'Très Forte';
                strengthClass = 'strength-4';
            }

            strengthDisplay.textContent = `Force du mot de passe : ${strengthText}`;
            strengthDisplay.className = `password-strength ${strengthClass}`;
        });
    </script>
</body>
</html>
