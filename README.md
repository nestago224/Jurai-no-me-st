# Jurai-no-me-st
```html
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Jurai no Me</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, sans-serif;
      background: #050505;
      color: white;
    }

    /* BARRE DE NAVIGATION */
    nav {
      position: fixed;
      top: 0;
      width: 100%;
      z-index: 1000;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 18px 7%;
      background: rgba(0, 0, 0, 0.85);
      border-bottom: 1px solid #222;
      backdrop-filter: blur(10px);
    }

    .logo {
      font-size: 25px;
      font-weight: bold;
      letter-spacing: 3px;
    }

    .logo span {
      color: #d00000;
    }

    nav ul {
      display: flex;
      gap: 30px;
      list-style: none;
    }

    nav a {
      color: white;
      text-decoration: none;
      font-weight: bold;
      transition: 0.3s;
    }

    nav a:hover {
      color: #e00000;
    }

    /* ACCUEIL */
    #accueil {
      min-height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 100px 20px 40px;
      background:
        linear-gradient(rgba(0,0,0,.55), rgba(0,0,0,.9)),
        url("images/fond.jpg") center/cover;
    }

    .hero {
      max-width: 900px;
    }

    .hero h1 {
      font-size: clamp(55px, 10vw, 120px);
      letter-spacing: 10px;
      text-transform: uppercase;
      text-shadow: 0 0 25px #900000;
    }

    .hero h1 span {
      color: #d00000;
    }

    .hero p {
      margin: 20px auto 35px;
      font-size: 20px;
      color: #ccc;
      max-width: 650px;
    }

    .btn {
      display: inline-block;
      padding: 14px 30px;
      margin: 5px;
      border: 1px solid #d00000;
      color: white;
      text-decoration: none;
      font-weight: bold;
      transition: .3s;
      background: rgba(120,0,0,.15);
    }

    .btn:hover {
      background: #d00000;
      box-shadow: 0 0 25px #d00000;
      transform: translateY(-3px);
    }

    /* SECTIONS */
    section {
      padding: 100px 8%;
    }

    .titre {
      text-align: center;
      font-size: 42px;
      margin-bottom: 50px;
      text-transform: uppercase;
    }

    .titre span {
      color: #d00000;
    }

    /* HISTOIRE */
    .histoire {
      max-width: 900px;
      margin: auto;
      line-height: 1.8;
      font-size: 18px;
      color: #ccc;
      text-align: center;
    }

    /* PERSONNAGES */
    .personnages {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
    }

    .carte {
      background: #101010;
      border: 1px solid #292929;
      overflow: hidden;
      transition: .4s;
    }

    .carte:hover {
      transform: translateY(-8px);
      border-color: #d00000;
      box-shadow: 0 10px 30px rgba(180,0,0,.25);
    }

    .carte img {
      width: 100%;
      height: 350px;
      object-fit: cover;
      display: block;
    }

    .carte-content {
      padding: 22px;
    }

    .carte h3 {
      font-size: 25px;
      margin-bottom: 10px;
    }

    .carte p {
      color: #aaa;
      line-height: 1.6;
    }

    /* GALERIE */
    .galerie {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 15px;
    }

    .galerie img {
      width: 100%;
      height: 280px;
      object-fit: cover;
      border: 1px solid #222;
      transition: .4s;
    }

    .galerie img:hover {
      transform: scale(1.03);
      border-color: #d00000;
    }

    /* FOOTER */
    footer {
      text-align: center;
      padding: 35px;
      background: #020202;
      border-top: 1px solid #222;
      color: #777;
    }

    footer span {
      color: #d00000;
    }

    /* MOBILE */
    @media (max-width: 700px) {
      nav {
        padding: 15px 20px;
      }

      nav ul {
        gap: 12px;
        font-size: 13px;
      }

      .hero h1 {
        letter-spacing: 5px;
      }

      section {
        padding: 80px 20px;
      }
    }
  </style>
</head>

<body>

  <nav>
    <div class="logo">JURAI <span>NO ME</span></div>

    <ul>
      <li><a href="#accueil">Accueil</a></li>
      <li><a href="#histoire">Histoire</a></li>
      <li><a href="#personnages">Personnages</a></li>
      <li><a href="#galerie">Galerie</a></li>
    </ul>
  </nav>


  <!-- ACCUEIL -->
  <section id="accueil">

    <div class="hero">
      <h1>Jurai <span>no Me</span></h1>

      <p>
        Bienvenue dans l'univers de Jurai no Me.
        Découvrez son histoire, ses personnages et les événements
        qui façonnent ce monde.
      </p>

      <a href="#histoire" class="btn">Découvrir l'histoire</a>
      <a href="#personnages" class="btn">Personnages</a>
    </div>

  </section>


  <!-- HISTOIRE -->
  <section id="histoire">

    <h2 class="titre">L'<span>histoire</span></h2>

    <div class="histoire">
      <p>
        Vingt ans après les événements de Jujutsu Kaisen, un nouveau monde
        commence à prendre forme. De nouveaux exorcistes apparaissent,
        tandis qu'une mystérieuse menace se rapproche dans l'ombre.
      </p>

      <br>

      <p>
        Parmi eux se trouve Kaku, un jeune exorciste dont le destin
        pourrait bouleverser l'équilibre du monde.
      </p>

      <br>

      <p>
        L'histoire de Jurai no Me ne fait que commencer...
      </p>
    </div>

  </section>


  <!-- PERSONNAGES -->
  <section id="personnages">

    <h2 class="titre">Les <span>personnages</span></h2>

    <div class="personnages">

      <div class="carte">
        <img src="images/kaku.jpg" alt="Kaku">
        <div class="carte-content">
          <h3>Kaku Kakuru</h3>
          <p>
            Un jeune exorciste mystérieux qui possède un destin
            particulier dans l'univers de Jurai no Me.
          </p>
        </div>
      </div>

      <div class="carte">
        <img src="images/yuji.jpg" alt="Yuji">
        <div class="carte-content">
          <h3>Yuji Itadori</h3>
          <p>
            Une figure importante de l'ancien monde,
            dont l'histoire continue d'avoir des conséquences.
          </p>
        </div>
      </div>

    </div>

  </section>


  <!-- GALERIE -->
  <section id="galerie">

    <h2 class="titre"><span>Galerie</span></h2>

    <div class="galerie">

      <img src="images/kaku.jpg" alt="Kaku">
      <img src="images/yuji.jpg" alt="Yuji">
      <img src="images/fond.jpg" alt="Jurai no Me">
      <img src="images/combat.jpg" alt="Combat">

    </div>

  </section>


  <footer>
    <p>© 2026 <span>Jurai no Me</span> — Fan project</p>
  </footer>

</body>
</html>
```

### 📁 Pour les images

Dans le même dossier que `index.html`, crée un dossier **`images`** et mets dedans :

```text
images/
├── fond.jpg
├── kaku.jpg
├── yuji.jpg
└── combat.jpg
```

Tu pourras remplacer ces images par **tes propres images de Kaku et Yuji**.

Si tu veux, je peux aussi te faire une **version beaucoup plus stylée**, avec une vraie page d'accueil de manga, des animations, un menu hamburger sur téléphone et les images de Kaku/Yuji directement intégrées. 🔥
