<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>TimValSecur V2</title>
  <style>
    /* Reset basique */
    * {
      margin: 0; padding: 0; box-sizing: border-box;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      color: #e0e0e0;
    }

    body {
      background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
      display: flex;
      min-height: 100vh;
      overflow-x: hidden;
    }

    /* Volet de navigation */
    nav {
      width: 280px;
      background: #12141dcc;
      backdrop-filter: blur(12px);
      padding: 2rem 1.5rem;
      display: flex;
      flex-direction: column;
      position: fixed;
      height: 100vh;
    }

    nav h1 {
      font-size: 1.8rem;
      margin-bottom: 2rem;
      color: #66fcf1;
      text-align: center;
      letter-spacing: 2px;
    }

    nav a {
      color: #66fcf1cc;
      text-decoration: none;
      margin: 0.8rem 0;
      font-weight: 600;
      transition: color 0.3s;
      border-left: 4px solid transparent;
      padding-left: 0.8rem;
    }

    nav a:hover,
    nav a.active {
      color: #45a29e;
      border-left: 4px solid #45a29e;
    }

    /* Contenu principal */
    main {
      margin-left: 280px;
      padding: 2rem 3rem;
      flex-grow: 1;
      overflow-y: auto;
    }

    section {
      margin-bottom: 4rem;
    }

    h2 {
      color: #45a29e;
      font-size: 2rem;
      margin-bottom: 1rem;
      border-bottom: 2px solid #45a29e;
      padding-bottom: 0.3rem;
      letter-spacing: 1px;
    }

    p {
      line-height: 1.6;
      font-size: 1.1rem;
      margin-bottom: 1rem;
      color: #cbd5e1;
    }

    code {
      background: #1f2833;
      padding: 2px 6px;
      border-radius: 4px;
      font-family: monospace;
      color: #66fcf1;
    }

    /* Zone test mot de passe */
    .password-test {
      background: #1f2833aa;
      padding: 1rem 1.5rem;
      border-radius: 10px;
      max-width: 400px;
      margin-top: 1rem;
    }

    .password-test input {
      width: 100%;
      padding: 0.6rem 1rem;
      border-radius: 6px;
      border: none;
      font-size: 1rem;
      margin-bottom: 0.8rem;
      outline: none;
    }

    .password-test button {
      background: #45a29e;
      color: #0b0c10;
      font-weight: 700;
      border: none;
      border-radius: 6px;
      padding: 0.6rem 1rem;
      cursor: pointer;
      width: 100%;
      transition: background 0.3s;
    }

    .password-test button:hover {
      background: #66fcf1;
    }

    .result {
      margin-top: 1rem;
      font-weight: 700;
      font-size: 1.1rem;
    }

    /* Footer avec boutons de liens */
    footer {
      position: fixed;
      bottom: 0;
      left: 280px;
      right: 0;
      background: #12141ddd;
      padding: 1rem 3rem;
      display: flex;
      justify-content: center;
      gap: 2rem;
      border-top: 1px solid #45a29e;
    }

    footer button {
      background: #0b0c10;
      border: 2px solid #45a29e;
      color: #45a29e;
      padding: 0.7rem 1.5rem;
      font-weight: 700;
      cursor: pointer;
      border-radius: 10px;
      transition: all 0.3s;
    }

    footer button:hover {
      background: #45a29e;
      color: #0b0c10;
      transform: scale(1.05);
    }

    /* Scrollbar stylée */
    main::-webkit-scrollbar {
      width: 8px;
    }

    main::-webkit-scrollbar-thumb {
      background: #45a29e88;
      border-radius: 10px;
    }

    main::-webkit-scrollbar-track {
      background: #0b0c10;
    }

    /* Responsive */
    @media (max-width: 768px) {
      nav {
        position: relative;
        width: 100%;
        height: auto;
        padding: 1rem;
        flex-direction: row;
        overflow-x: auto;
      }
      nav h1 {
        flex: 1;
        margin-bottom: 0;
        text-align: left;
      }
      nav a {
        margin: 0 1rem;
        border-left: none;
        padding-left: 0;
        white-space: nowrap;
      }
      main {
        margin-left: 0;
        padding: 1rem;
      }
      footer {
        left: 0;
        right: 0;
        padding: 1rem;
      }
    }
  </style>
</head>
<body>
  <nav>
    <h1>TimValSecur V2</h1>
    <a href="#pirates" class="active">Les Pirates</a>
    <a href="#traqueurs">Les Traqueurs</a>
    <a href="#test-mdp">Tester son Mot de Passe</a>
    <a href="#prevention">Prévention</a>
  </nav>

  <main>
    <section id="pirates">
      <h2>Les Pirates</h2>
      <p>
        Les pirates informatiques sont des personnes qui cherchent à accéder illégalement à des systèmes informatiques. Ils utilisent diverses techniques comme le phishing, les malwares, les failles de sécurité ou encore le social engineering pour compromettre vos données.
      </p>
      <p>
        Leur but peut être de voler des informations sensibles, de détruire des données, ou simplement de perturber des services.
      </p>
    </section>

    <section id="traqueurs">
      <h2>Les Traqueurs</h2>
      <p>
        Les traqueurs sont des programmes, souvent sous forme de cookies ou scripts, qui collectent vos données de navigation à votre insu. Ils peuvent suivre votre activité sur plusieurs sites pour construire un profil marketing ou même compromettre votre vie privée.
      </p>
      <p>
        Il est important de comprendre comment fonctionnent ces traqueurs pour mieux se protéger en utilisant des extensions anti-tracking et en configurant correctement la confidentialité de votre navigateur.
      </p>
    </section>

    <section id="test-mdp">
      <h2>Tester son Mot de Passe</h2>
      <p>
        Un mot de passe fort est la première ligne de défense contre le piratage. Utilisez des combinaisons longues, incluant lettres, chiffres, et symboles. Vous pouvez tester la robustesse de votre mot de passe ici :
      </p>
      <div class="password-test">
        <input type="password" id="passwordInput" placeholder="Entrez votre mot de passe" />
        <button onclick="testPassword()">Tester</button>
        <div id="result" class="result"></div>
      </div>
    </section>

    <section id="prevention">
      <h2>Comment ne pas se faire pirater</h2>
      <p>
        Voici quelques conseils pour éviter de vous faire pirater :
      </p>
      <ul>
        <li>Utilisez des mots de passe forts et uniques pour chaque service.</li>
        <li>Activez l'authentification à deux facteurs (2FA) quand c’est possible.</li>
        <li>Méfiez-vous des emails et liens suspects (phishing).</li>
        <li>Gardez vos logiciels et systèmes à jour.</li>
        <li>Utilisez un gestionnaire de mots de passe pour sécuriser vos identifiants.</li>
        <li>Évitez de cliquer sur des publicités ou fichiers inconnus.</li>
      </ul>
    </section>
  </main>

  <footer>
    <button onclick="window.open('https://haveibeenpwned.com/', '_blank')">Check Pwned</button>
    <button onclick="window.open('https://www.cybermalveillance.gouv.fr/', '_blank')">Cybermalveillance</button>
    <button onclick="window.open('https://tiboval.github.io/Timval-Secur-conexion/')">conexion</button>
  </footer>

  <script>
    // Gestion active link dans le menu (au scroll)
    const sections = document.querySelectorAll("main section");
    const navLinks = document.querySelectorAll("nav a");

    window.addEventListener("scroll", () => {
      let current = "";
      sections.forEach((section) => {
        const sectionTop = section.offsetTop - 100;
        if (pageYOffset >= sectionTop) {
          current = section.getAttribute("id");
        }
      });

      navLinks.forEach((link) => {
        link.classList.remove("active");
        if (link.getAttribute("href") === "#" + current) {
          link.classList.add("active");
        }
      });
    });

    // Fonction simple pour tester un mot de passe
    function testPassword() {
      const pwd = document.getElementById("passwordInput").value;
      const result = document.getElementById("result");
      if (!pwd) {
        result.textContent = "Veuillez entrer un mot de passe.";
        result.style.color = "#ff5555";
        return;
      }

      let score = 0;

      // Longueur
      if (pwd.length >= 8) score += 1;
      if (pwd.length >= 12) score += 1;

      // Lettres majuscules et minuscules
      if (/[a-z]/.test(pwd) && /[A-Z]/.test(pwd)) score += 1;

      // Chiffres
      if (/\d/.test(pwd)) score += 1;

      // Symboles
      if (/[\W_]/.test(pwd)) score += 1;

      // Résultat simple
      if (score <= 1) {
        result.textContent = "Mot de passe très faible 🔴";
        result.style.color = "#ff4444";
      } else if (score === 2 || score === 3) {
        result.textContent = "Mot de passe moyen 🟠";
        result.style.color = "#ffae42";
      } else if (score >= 4) {
        result.textContent = "Mot de passe fort 🟢";
        result.style.color = "#45a29e";
      }
    }
  </script>
</body>
</html>

