[recrutement-closers-setters-ia (7).html](https://github.com/user-attachments/files/29388456/recrutement-closers-setters-ia.7.html)
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Recrutement Closers & Setters — Formation IA CPF</title>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700;800;900&family=Inter:wght@400;500;600&display=swap" rel="stylesheet" />
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

    :root {
      --navy: #0D1B2A;
      --navy-mid: #132032;
      --navy-light: #1A2E45;
      --blue: #2563EB;
      --blue-light: #3B82F6;
      --gold: #F59E0B;
      --gold-light: #FCD34D;
      --white: #F8FAFC;
      --muted: #94A3B8;
      --border: rgba(255,255,255,0.08);
      --radius: 12px;
    }

    html { scroll-behavior: smooth; }

    body {
      font-family: 'Inter', sans-serif;
      background: var(--navy);
      color: var(--white);
      line-height: 1.7;
      min-height: 100vh;
    }

    /* ─── NAV ─── */
    nav {
      position: fixed; top: 0; width: 100%; z-index: 100;
      background: rgba(13,27,42,0.92);
      backdrop-filter: blur(12px);
      border-bottom: 1px solid var(--border);
      padding: 1rem 2rem;
      display: flex; align-items: center; justify-content: space-between;
    }
    .logo { font-family: 'Playfair Display', serif; font-size: 1.2rem; font-weight: 800; letter-spacing: -0.02em; }
    .logo span { color: var(--gold); }
    .nav-badge {
      background: rgba(245,158,11,0.15);
      color: var(--gold);
      border: 1px solid rgba(245,158,11,0.3);
      border-radius: 999px;
      font-size: 0.75rem;
      font-weight: 600;
      padding: 4px 14px;
      letter-spacing: 0.05em;
    }

    /* ─── HERO ─── */
    .hero {
      padding: 9rem 2rem 5rem;
      max-width: 860px;
      margin: 0 auto;
      text-align: center;
    }
    .hero-eyebrow {
      display: inline-flex; align-items: center; gap: 8px;
      background: rgba(37,99,235,0.15);
      border: 1px solid rgba(37,99,235,0.35);
      border-radius: 999px;
      color: #93C5FD;
      font-size: 0.78rem;
      font-weight: 600;
      letter-spacing: 0.08em;
      padding: 6px 18px;
      margin-bottom: 2rem;
      text-transform: uppercase;
    }
    .dot { width: 7px; height: 7px; border-radius: 50%; background: #22C55E; animation: pulse 1.8s ease-in-out infinite; }
    @keyframes pulse { 0%,100%{opacity:1;transform:scale(1)} 50%{opacity:0.5;transform:scale(0.7)} }

    h1 {
      font-family: 'Playfair Display', serif;
      font-size: clamp(2.4rem, 6vw, 4rem);
      font-weight: 800;
      line-height: 1.1;
      letter-spacing: -0.03em;
      margin-bottom: 1.5rem;
    }
    h1 .accent { color: var(--gold); }
    h1 .accent-blue { color: #60A5FA; }

    .hero-sub {
      font-size: 1.1rem;
      color: var(--muted);
      max-width: 600px;
      margin: 0 auto 2.5rem;
      line-height: 1.75;
    }

    /* ─── URGENCE BAR ─── */
    .urgence-bar {
      background: var(--navy-light);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 1.2rem 1.5rem;
      max-width: 500px;
      margin: 0 auto 3.5rem;
    }
    .urgence-label {
      display: flex; justify-content: space-between; align-items: center;
      font-size: 0.82rem; color: var(--muted); margin-bottom: 10px;
    }
    .urgence-label strong { color: var(--gold); font-weight: 600; }
    .bar-track {
      height: 8px; background: rgba(255,255,255,0.08); border-radius: 999px; overflow: hidden;
    }
    .bar-fill {
      height: 100%; border-radius: 999px;
      background: linear-gradient(90deg, #F59E0B, #EF4444);
      width: 0; animation: fillbar 1.4s ease-out 0.6s forwards;
    }
    @keyframes fillbar { to { width: 74%; } }

    /* ─── STATS ─── */
    .stats {
      display: flex; flex-wrap: wrap; justify-content: center; gap: 1rem;
      margin-bottom: 5rem; padding: 0 1rem;
    }
    .stat-card {
      background: var(--navy-light);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 1.4rem 2rem;
      text-align: center;
      flex: 1; min-width: 160px; max-width: 200px;
    }
    .stat-num {
      font-family: 'Playfair Display', serif;
      font-size: 2rem; font-weight: 800;
      color: var(--gold); line-height: 1;
      margin-bottom: 4px;
    }
    .stat-label { font-size: 0.78rem; color: var(--muted); }

    /* ─── SECTION TITLE ─── */
    .section { padding: 4rem 1.5rem; max-width: 960px; margin: 0 auto; }
    .section-title {
      font-family: 'Playfair Display', serif;
      font-size: clamp(1.5rem, 3.5vw, 2.2rem);
      font-weight: 800;
      letter-spacing: -0.02em;
      text-align: center;
      margin-bottom: 0.5rem;
    }
    .section-sub {
      text-align: center; color: var(--muted); font-size: 0.95rem;
      margin-bottom: 2.5rem;
    }

    /* ─── RÔLES ─── */
    .roles-grid {
      display: grid; grid-template-columns: 1fr 1fr; gap: 1.5rem;
      margin-bottom: 2rem;
    }
    @media(max-width:640px){ .roles-grid { grid-template-columns: 1fr; } }

    .role-card {
      background: var(--navy-light);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 2rem;
      position: relative; overflow: hidden;
      transition: border-color 0.2s;
    }
    .role-card:hover { border-color: rgba(37,99,235,0.5); }
    .role-card::before {
      content:''; position:absolute; top:0; left:0; right:0; height:3px;
    }
    .role-card.closer::before { background: linear-gradient(90deg, #2563EB, #60A5FA); }
    .role-card.setter::before { background: linear-gradient(90deg, #F59E0B, #FCD34D); }

    .role-icon {
      width: 44px; height: 44px; border-radius: 10px;
      display: flex; align-items: center; justify-content: center;
      font-size: 1.3rem; margin-bottom: 1rem;
    }
    .closer .role-icon { background: rgba(37,99,235,0.18); }
    .setter .role-icon { background: rgba(245,158,11,0.18); }

    .role-title {
      font-family: 'Playfair Display', serif;
      font-size: 1.15rem; font-weight: 800;
      margin-bottom: 0.5rem;
    }
    .role-tag {
      display: inline-block;
      font-size: 0.7rem; font-weight: 600;
      border-radius: 999px; padding: 3px 10px;
      margin-bottom: 0.8rem;
      letter-spacing: 0.05em;
    }
    .closer .role-tag { background: rgba(37,99,235,0.18); color: #93C5FD; }
    .setter .role-tag { background: rgba(245,158,11,0.18); color: #FCD34D; }

    .role-desc { font-size: 0.88rem; color: var(--muted); margin-bottom: 1rem; line-height: 1.6; }

    .role-perks { list-style: none; display: flex; flex-direction: column; gap: 6px; }
    .role-perks li {
      font-size: 0.83rem; color: #CBD5E1;
      display: flex; align-items: flex-start; gap: 8px;
    }
    .role-perks li::before { content: '✓'; color: #22C55E; font-weight: 700; flex-shrink:0; margin-top:1px; }

    /* ─── FORMATION BLOCK ─── */
    .formation-block {
      background: var(--navy-light);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 2rem;
      margin-bottom: 4rem;
    }
    .formation-header {
      display: flex; align-items: center; gap: 12px; margin-bottom: 1.5rem;
    }
    .cpf-badge {
      background: linear-gradient(135deg, #059669, #10B981);
      color: #fff;
      font-size: 0.7rem; font-weight: 700;
      letter-spacing: 0.08em;
      padding: 5px 12px; border-radius: 6px;
    }
    .formation-title { font-family: 'Playfair Display', serif; font-size: 1.1rem; font-weight: 800; }
    .modules-grid {
      display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 1rem;
    }
    .module {
      background: rgba(255,255,255,0.04);
      border: 1px solid var(--border);
      border-radius: 8px; padding: 1rem 1.2rem;
    }
    .module-num { font-size: 0.7rem; color: #60A5FA; font-weight: 700; letter-spacing: 0.1em; margin-bottom: 4px; }
    .module-name { font-size: 0.87rem; font-weight: 500; color: var(--white); }

    /* ─── FORM ─── */
    .form-section {
      background: var(--navy-mid);
      border-top: 1px solid var(--border);
      padding: 5rem 1.5rem;
    }
    .form-wrap {
      max-width: 600px; margin: 0 auto;
    }
    .form-card {
      background: var(--navy-light);
      border: 1px solid var(--border);
      border-radius: 16px;
      padding: 2.5rem;
    }
    .form-title {
      font-family: 'Playfair Display', serif;
      font-size: 1.6rem; font-weight: 800;
      text-align: center; margin-bottom: 0.4rem;
    }
    .form-sub {
      text-align: center; color: var(--muted); font-size: 0.88rem;
      margin-bottom: 2rem;
    }

    .form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 1rem; margin-bottom: 1rem; }
    @media(max-width:480px){ .form-row { grid-template-columns: 1fr; } }

    .field { display: flex; flex-direction: column; gap: 6px; margin-bottom: 1rem; }
    .field:last-of-type { margin-bottom: 0; }

    label { font-size: 0.82rem; font-weight: 600; color: #CBD5E1; }
    label span { color: #EF4444; margin-left: 2px; }

    input, select, textarea {
      background: rgba(255,255,255,0.05);
      border: 1px solid rgba(255,255,255,0.12);
      border-radius: 8px;
      color: var(--white);
      font-family: 'Inter', sans-serif;
      font-size: 0.9rem;
      padding: 0.7rem 1rem;
      outline: none;
      transition: border-color 0.2s, box-shadow 0.2s;
      width: 100%;
    }
    input::placeholder, textarea::placeholder { color: #475569; }
    input:focus, select:focus, textarea:focus {
      border-color: var(--blue-light);
      box-shadow: 0 0 0 3px rgba(37,99,235,0.18);
    }
    select option { background: var(--navy-mid); color: var(--white); }
    textarea { resize: vertical; min-height: 90px; }

    .role-select-group {
      display: grid; grid-template-columns: 1fr 1fr; gap: 0.8rem;
      margin-bottom: 1rem;
    }
    @media(max-width:480px){ .role-select-group { grid-template-columns: 1fr; } }

    .role-option {
      display: none;
    }
    .role-label {
      display: flex; align-items: center; justify-content: center; gap: 8px;
      padding: 0.7rem 1rem;
      border: 1px solid rgba(255,255,255,0.12);
      border-radius: 8px;
      font-size: 0.85rem; font-weight: 600;
      cursor: pointer;
      transition: all 0.2s;
      text-align: center;
    }
    .role-label:hover { border-color: rgba(255,255,255,0.25); background: rgba(255,255,255,0.04); }
    #role-closer:checked ~ .role-select-group label[for="role-closer"] {
      border-color: var(--blue); background: rgba(37,99,235,0.18); color: #93C5FD;
    }
    #role-setter:checked ~ .role-select-group label[for="role-setter"] {
      border-color: var(--gold); background: rgba(245,158,11,0.18); color: #FCD34D;
    }
    #role-both:checked ~ .role-select-group label[for="role-both"] {
      border-color: #22C55E; background: rgba(34,197,94,0.18); color: #86EFAC;
    }
    .role-option:checked + .role-label { font-weight: 700; }

    .submit-btn {
      display: block; width: 100%;
      background: linear-gradient(135deg, var(--blue), #1D4ED8);
      color: #fff;
      font-family: 'Playfair Display', serif;
      font-size: 1rem; font-weight: 700;
      padding: 1rem;
      border: none; border-radius: 10px;
      cursor: pointer;
      margin-top: 1.5rem;
      transition: transform 0.15s, box-shadow 0.2s;
      letter-spacing: 0.01em;
    }
    .submit-btn:hover {
      transform: translateY(-1px);
      box-shadow: 0 8px 24px rgba(37,99,235,0.35);
    }
    .submit-btn:active { transform: scale(0.98); }

    .form-legal {
      text-align: center; font-size: 0.72rem; color: #475569;
      margin-top: 1rem; line-height: 1.5;
    }

    /* ─── SUCCESS ─── */
    .success-msg {
      display: none; text-align: center; padding: 2rem;
    }
    .success-icon {
      width: 64px; height: 64px;
      background: rgba(34,197,94,0.15);
      border: 2px solid #22C55E;
      border-radius: 50%;
      display: flex; align-items: center; justify-content: center;
      font-size: 1.8rem;
      margin: 0 auto 1.5rem;
    }
    .success-title { font-family: 'Playfair Display', serif; font-size: 1.4rem; font-weight: 800; margin-bottom: 0.5rem; }
    .success-text { color: var(--muted); font-size: 0.9rem; }

    /* ─── FOOTER ─── */
    footer {
      text-align: center;
      padding: 2rem;
      color: #334155;
      font-size: 0.78rem;
      border-top: 1px solid var(--border);
    }

    /* ─── SCROLL REVEAL ─── */
    .reveal { opacity: 0; transform: translateY(24px); transition: opacity 0.6s ease, transform 0.6s ease; }
    .reveal.visible { opacity: 1; transform: translateY(0); }
  </style>
</head>
<body>

<!-- NAV -->
<nav>
  <div class="logo">IA<span>Vente</span>Pro</div>
  <div class="nav-badge">🟢 Recrutement ouvert</div>
</nav>

<!-- HERO -->
<section class="hero">
  <div class="hero-eyebrow">
    <span class="dot"></span>
    Opportunité indépendante — Formation éligible CPF
  </div>

  <h1>
    Vends la formation qui<br>
    <span class="accent">transforme les ventes</span><br>
    grâce à <span class="accent-blue">l'Intelligence Artificielle</span>
  </h1>

  <p class="hero-sub">
    Nous recrutons des <strong>closers</strong> et des <strong>setters</strong> indépendants passionnés
    par l'IA pour commercialiser notre formation certifiante CPF — 100% prise en charge,
    commissions attractives, liberté totale.
  </p>

  <div class="urgence-bar">
    <div class="urgence-label">
      <span>Places disponibles cette semaine</span>
      <strong>26 / 35 prises</strong>
    </div>
    <div class="bar-track"><div class="bar-fill"></div></div>
  </div>

  <div class="stats">
    <div class="stat-card">
      <div class="stat-num">100%</div>
      <div class="stat-label">Pris en charge CPF</div>
    </div>
    <div class="stat-card">
      <div class="stat-num">300 €</div>
      <div class="stat-label">Comm. par vente</div>
    </div>
    <div class="stat-card">
      <div class="stat-num">Indép.</div>
      <div class="stat-label">Liberté & flexibilité</div>
    </div>
    <div class="stat-card">
      <div class="stat-num">IA</div>
      <div class="stat-label">Marché en explosion</div>
    </div>
  </div>
</section>

<!-- RÔLES -->
<section class="section reveal">
  <div class="section-title">Quel rôle te correspond ?</div>
  <p class="section-sub">Deux profils recrutés, deux missions complémentaires</p>

  <div class="roles-grid">
    <div class="role-card closer">
      <div class="role-icon">🎯</div>
      <div class="role-title">Closer</div>
      <div class="role-tag">CLOSER</div>
      <p class="role-desc">
        Tu prends en charge les prospects qualifiés et tu concluies les ventes en appel vidéo.
        Maîtrise de l'écoute active, gestion des objections et closing haut ticket.
      </p>
      <ul class="role-perks">
        <li>Appels entrants qualifiés fournis par les setters</li>
        <li>Scripts et supports de vente inclus</li>
        <li>Formation au closing IA offerte</li>
        <li>Commission de 300 € par vente conclue</li>
        <li>Objectif atteignable : 5 à 15 ventes/mois</li>
      </ul>
    </div>

    <div class="role-card setter">
      <div class="role-icon">📱</div>
      <div class="role-title">Setter</div>
      <div class="role-tag">SETTER</div>
      <p class="role-desc">
        Tu génères et qualifies les leads via les réseaux sociaux, tu prends les rendez-vous
        et transmets les prospects chauds aux closers.
      </p>
      <ul class="role-perks">
        <li>Prospection via LinkedIn, Instagram, Meta Ads</li>
        <li>Scripts de qualification fournis</li>
        <li>CRM et outils IA mis à disposition</li>
        <li>Commission de 75 euros à la conversion</li>
        <li>Évolution vers poste closer possible</li>
      </ul>
    </div>
  </div>
</section>

<!-- FORMATION -->
<section class="section reveal" style="padding-top:0;">
  <div class="section-title">La formation que tu vas vendre</div>
  <p class="section-sub">Éligible CPF · 100% financée · En forte demande</p>

  <div class="formation-block">
    <div class="formation-header">
      <span class="cpf-badge">✓ ÉLIGIBLE CPF</span>
      <span class="formation-title">Intégrer l'IA dans son cycle de vente & marketing de contenu</span>
    </div>

    <div class="modules-grid">
      <div class="module">
        <div class="module-num">MODULE 01</div>
        <div class="module-name">IA appliquée aux cycles de vente</div>
      </div>
      <div class="module">
        <div class="module-num">MODULE 02</div>
        <div class="module-name">Prospection augmentée par l'IA</div>
      </div>
      <div class="module">
        <div class="module-num">MODULE 03</div>
        <div class="module-name">Marketing de contenu avec l'IA</div>
      </div>
      <div class="module">
        <div class="module-num">MODULE 04</div>
        <div class="module-name">Développer son activité pro avec l'IA</div>
      </div>
      <div class="module">
        <div class="module-num">MODULE 05</div>
        <div class="module-name">Automatisation & outils IA terrain</div>
      </div>
      <div class="module">
        <div class="module-num">MODULE 06</div>
        <div class="module-name">Certification</div>
      </div>
    </div>
  </div>
</section>

<!-- FORMULAIRE -->
<section class="form-section">
  <div class="form-wrap reveal">
    <div class="section-title" style="margin-bottom:0.4rem;">Rejoins l'équipe</div>
    <p class="section-sub" style="margin-bottom:2rem;">Remplis le formulaire — notre équipe te contacte sous 24h</p>

    <div class="form-card">

      <!-- FORMULAIRE -->
      <div id="contact-form">
        <p class="form-title" style="font-size:1.2rem; margin-bottom:0.3rem;">Ta candidature</p>
        <p class="form-sub">Tous les champs sont obligatoires</p>

        <div class="form-row">
          <div class="field">
            <label for="prenom">Prénom <span>*</span></label>
            <input type="text" id="prenom" placeholder="Marie" autocomplete="given-name" required />
          </div>
          <div class="field">
            <label for="nom">Nom <span>*</span></label>
            <input type="text" id="nom" placeholder="Dupont" autocomplete="family-name" required />
          </div>
        </div>

        <div class="field">
          <label for="email">Adresse e-mail <span>*</span></label>
          <input type="email" id="email" placeholder="marie.dupont@email.com" autocomplete="email" required />
        </div>

        <div class="field">
          <label for="whatsapp">Numéro WhatsApp <span>*</span></label>
          <input type="tel" id="whatsapp" placeholder="+33 6 12 34 56 78" autocomplete="tel" required />
        </div>

        <div class="field">
          <label>Rôle souhaité <span>*</span></label>
          <div style="display:grid; grid-template-columns:1fr 1fr 1fr; gap:0.7rem; margin-top:4px;">
            <label for="r-closer" id="btn-closer" style="display:flex;align-items:center;justify-content:center;gap:6px;padding:0.65rem;border:1px solid rgba(255,255,255,0.12);border-radius:8px;font-size:0.83rem;font-weight:600;cursor:pointer;transition:all 0.2s;">
              <input type="radio" id="r-closer" name="role" value="closer" style="display:none;" />
              🎯 Closer
            </label>
            <label for="r-setter" id="btn-setter" style="display:flex;align-items:center;justify-content:center;gap:6px;padding:0.65rem;border:1px solid rgba(255,255,255,0.12);border-radius:8px;font-size:0.83rem;font-weight:600;cursor:pointer;transition:all 0.2s;">
              <input type="radio" id="r-setter" name="role" value="setter" style="display:none;" />
              📱 Setter
            </label>
            <label for="r-both" id="btn-both" style="display:flex;align-items:center;justify-content:center;gap:6px;padding:0.65rem;border:1px solid rgba(255,255,255,0.12);border-radius:8px;font-size:0.83rem;font-weight:600;cursor:pointer;transition:all 0.2s;">
              <input type="radio" id="r-both" name="role" value="both" style="display:none;" />
              🔥 Les deux
            </label>
          </div>
        </div>

        <div class="field">
          <label for="experience">Ton expérience en vente <span>*</span></label>
          <select id="experience" required>
            <option value="" disabled selected>Sélectionne ton niveau</option>
            <option value="debutant">Débutant — moins de 6 mois</option>
            <option value="intermediaire">Intermédiaire — 6 mois à 2 ans</option>
            <option value="confirme">Confirmé — 2 à 5 ans</option>
            <option value="expert">Expert — plus de 5 ans</option>
          </select>
        </div>

        <div class="field" style="margin-bottom:0;">
          <label for="motivation">Pourquoi rejoindre notre équipe ? <span>*</span></label>
          <textarea id="motivation" placeholder="Parle-nous de ta motivation, de ton expérience et de ce que l'IA représente pour toi..." required></textarea>
        </div>

        <button class="submit-btn" onclick="handleSubmit()">
          Envoyer ma candidature →
        </button>

        <p class="form-legal">
          En soumettant ce formulaire, tu acceptes d'être contacté par notre équipe
          par e-mail ou WhatsApp. Aucun spam, promis.
        </p>
      </div>

      <!-- SUCCESS -->
      <div class="success-msg" id="success-msg">
        <div class="success-icon">✓</div>
        <div class="success-title">Candidature envoyée !</div>
        <p class="success-text" style="margin-top:0.5rem;">
          Merci pour ta motivation 🎉<br>
          Notre équipe te contactera dans les <strong style="color:var(--gold)">24 heures</strong>
          sur WhatsApp ou par e-mail pour un premier échange.
        </p>
      </div>

    </div>
  </div>
</section>

<footer>
  © 2025 IAVentePro — Formation éligible CPF · Tous droits réservés
</footer>

<script>
  // ─── Scroll reveal ───
  const reveals = document.querySelectorAll('.reveal');
  const observer = new IntersectionObserver(entries => {
    entries.forEach(e => { if (e.isIntersecting) { e.target.classList.add('visible'); } });
  }, { threshold: 0.1 });
  reveals.forEach(r => observer.observe(r));

  // ─── Role radio styling ───
  const roleButtons = {
    'r-closer': { btn: 'btn-closer', color: 'rgba(37,99,235,0.22)', border: '#3B82F6', text: '#93C5FD' },
    'r-setter': { btn: 'btn-setter', color: 'rgba(245,158,11,0.22)', border: '#F59E0B', text: '#FCD34D' },
    'r-both':   { btn: 'btn-both',   color: 'rgba(34,197,94,0.22)',  border: '#22C55E', text: '#86EFAC' },
  };
  document.querySelectorAll('input[name="role"]').forEach(radio => {
    radio.addEventListener('change', () => {
      Object.values(roleButtons).forEach(v => {
        const el = document.getElementById(v.btn);
        el.style.background = '';
        el.style.borderColor = 'rgba(255,255,255,0.12)';
        el.style.color = '';
      });
      const cfg = roleButtons[radio.id];
      const lbl = document.getElementById(cfg.btn);
      lbl.style.background = cfg.color;
      lbl.style.borderColor = cfg.border;
      lbl.style.color = cfg.text;
    });
  });

  // ─── Submit ───
  async function handleSubmit() {
    const prenom = document.getElementById('prenom').value.trim();
    const nom = document.getElementById('nom').value.trim();
    const email = document.getElementById('email').value.trim();
    const whatsapp = document.getElementById('whatsapp').value.trim();
    const role = document.querySelector('input[name="role"]:checked');
    const experience = document.getElementById('experience').value;
    const motivation = document.getElementById('motivation').value.trim();

    if (!prenom || !nom || !email || !whatsapp || !role || !experience || !motivation) {
      const fields = [
        [prenom,'prenom'],[nom,'nom'],[email,'email'],
        [whatsapp,'whatsapp'],[experience,'experience'],[motivation,'motivation']
      ];
      fields.forEach(([val, id]) => {
        const el = document.getElementById(id);
        if (!val) { el.style.borderColor = '#EF4444'; } else { el.style.borderColor = ''; }
      });
      if (!role) { document.getElementById('btn-closer').style.borderColor = '#EF4444'; }
      return;
    }

    const btn = document.querySelector('.submit-btn');
    btn.textContent = 'Envoi en cours…';
    btn.disabled = true;

    try {
      const res = await fetch('https://formspree.io/f/xvzjaayp', {
        method: 'POST',
        headers: { 'Content-Type': 'application/json', 'Accept': 'application/json' },
        body: JSON.stringify({
          _replyto: email,
          _subject: 'Nouvelle candidature — ' + prenom + ' ' + nom,
          Prenom: prenom,
          Nom: nom,
          Email: email,
          WhatsApp: whatsapp,
          Role: role.value,
          Experience: experience,
          Motivation: motivation
        })
      });

      if (res.ok) {
        document.getElementById('contact-form').style.display = 'none';
        document.getElementById('success-msg').style.display = 'block';
      } else {
        btn.textContent = 'Envoyer ma candidature →';
        btn.disabled = false;
        alert('Une erreur est survenue. Merci de reessayer.');
      }
    } catch(err) {
      btn.textContent = 'Envoyer ma candidature →';
      btn.disabled = false;
      alert('Impossible d envoyer. Verifiez votre connexion.');
    }
  }
</script>
</body>
</html>
