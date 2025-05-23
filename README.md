# Les Voyages Malins de Vic

Site de conseils de voyage façon carnet de route.
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Les Voyages Malins de Vic</title>
  <style>
    body {
      font-family: 'Georgia', serif;
      background: url('https://www.transparenttextures.com/patterns/paper-fibers.png');
      color: #4b3f2f;
      margin: 0;
      padding-top: 60px;
    }
    nav {
      background-color: #fff7ec;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      display: flex;
      justify-content: center;
      padding: 1rem;
      z-index: 999;
    }
    nav a {
      margin: 0 1rem;
      text-decoration: none;
      color: #4b3f2f;
      font-weight: bold;
    }
    nav a:hover {
      color: #c28f2c;
    }
    h1 {
      font-size: 3rem;
      text-align: center;
      margin-bottom: 0.5rem;
    }
    p {
      text-align: center;
      font-style: italic;
      color: #6b5b3e;
      margin-bottom: 2rem;
    }
    section {
      max-width: 900px;
      margin: 0 auto;
      padding: 0 1rem;
    }
    .box {
      background: rgba(255, 255, 255, 0.8);
      padding: 1.5rem;
      margin-bottom: 1.5rem;
      border-radius: 1rem;
      box-shadow: 2px 2px 10px rgba(0,0,0,0.1);
    }
    .box h2 {
      font-size: 1.5rem;
      margin-bottom: 0.75rem;
    }
    ul {
      padding-left: 1.2rem;
    }
    ul li {
      margin-bottom: 0.5rem;
    }
    .service-links {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      margin-top: 1rem;
    }
    .service-links a {
      flex: 1 1 calc(50% - 1rem);
      background: #fff;
      border: 2px solid #dec9a5;
      border-radius: 10px;
      text-align: center;
      padding: 1rem;
      text-decoration: none;
      color: #4b3f2f;
      font-weight: bold;
      transition: 0.3s ease;
    }
    .service-links a:hover {
      background-color: #f5e7c1;
      transform: translateY(-3px);
    }
    form {
      display: flex;
      flex-direction: column;
      gap: 1rem;
      margin-top: 1rem;
    }
    form label {
      font-weight: bold;
    }
    form input, form textarea, form select {
      padding: 0.5rem;
      border: 1px solid #ccc;
      border-radius: 5px;
      font-family: inherit;
    }
    form button {
      background-color: #c28f2c;
      color: white;
      padding: 0.75rem;
      border: none;
      border-radius: 5px;
      font-size: 1rem;
      cursor: pointer;
    }
    form button:hover {
      background-color: #a8741c;
    }
  </style>
</head>
<body>
  <nav>
    <a href="#accueil">Accueil</a>
    <a href="#destinations">Destinations</a>
    <a href="#conseils">Conseils</a>
    <a href="#carnet">Carnet</a>
    <a href="#services">Services</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="accueil">
    <h1>Les Voyages Malins de Vic</h1>
    <p>Carnet de route, bons plans et récits malins autour du monde</p>
  </section>

  <section id="destinations" class="box">
    <h2>Destinations</h2>
    <ul>
      <li>🌴 Malaisie</li>
      <li>🇮🇹 Pouilles (Italie)</li>
      <li>✈️ À venir...</li>
    </ul>
  </section>

  <section id="conseils" class="box">
    <h2>Conseils malins</h2>
    <ul>
      <li>Voyager léger mais bien équipé</li>
      <li>Applis indispensables en voyage</li>
      <li>Gérer son budget au quotidien</li>
    </ul>
  </section>

  <section id="carnet" class="box">
    <h2>Carnet de bord</h2>
    <p>Retrouve ici mes récits de voyage, mes galères, mes émerveillements et les petites astuces apprises sur la route. Prochainement : mes aventures en van dans les Pouilles et mon trip en sac à dos en Malaisie !</p>
  </section>

  <section id="services" class="box">
    <h2>Services</h2>
    <div class="service-links">
      <a href="#formulaire">🔍 Conseils personnalisés</a>
      <a href="#">🗓️ Prendre un rendez-vous</a>
      <a href="#">🚒 Checklists & matériel</a>
      <a href="#">📲 Partager mes réseaux sociaux</a>
    </div>
  </section>

  <section id="formulaire" class="box">
    <h2>Demande de conseils personnalisés</h2>
    <form action="https://formspree.io/f/xqkrdnez" method="POST">
      <label for="nom">Prénom / Nom</label>
      <input type="text" id="nom" name="nom" required>

      <label for="email">Adresse email</label>
      <input type="email" id="email" name="email" required>

      <label for="budget">Budget estimé (€)</label>
      <input type="number" id="budget" name="budget">

      <label for="personnes">Nombre de personnes</label>
      <input type="number" id="personnes" name="personnes">

      <label for="type">Type de voyage rêvé</label>
      <select id="type" name="type">
        <option value="">-- Choisir --</option>
        <option value="plage">Plage</option>
        <option value="aventure">Aventure</option>
        <option value="nature">Nature</option>
        <option value="culture">Culture</option>
        <option value="vanlife">Van life</option>
        <option value="autre">Autre</option>
      </select>

      <label for="destinations">Destinations envisagées</label>
      <textarea id="destinations" name="destinations" rows="2"></textarea>

      <label for="anciens">Voyages déjà réalisés</label>
      <textarea id="anciens" name="anciens" rows="2"></textarea>

      <label for="message">Message complémentaire (optionnel)</label>
      <textarea id="message" name="message" rows="3"></textarea>

      <button type="submit">Recevoir mes conseils personnalisés</button>
    <input type="hidden" name="_next" value="https://vicvoyage.github.io/les-voyages-de-vic/#formulaire">
      <p style="font-style:italic; font-size:0.9rem; color:#4b3f2f;">Une fois envoyé, tu recevras une réponse directement par email !</p>
    </form>
  </section>

  <section id="contact" class="box">
    <h2>Contact</h2>
    <p>Tu veux me poser une question ou me proposer un projet ? Écris-moi sur Instagram ou via un petit formulaire (bientôt dispo) !</p>
  </section>

</body>
</html>
