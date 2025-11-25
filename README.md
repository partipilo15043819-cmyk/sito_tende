<!DOCTYPE html>
<html lang="it">
<head>
  <meta charset="UTF-8">
  <title>Tendidea - Catalogo tende e zanzariere | Acquista online</title>
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <meta name="description" content="Tendidea - Vendita online di tende, zanzariere e accessori. Acquista in sicurezza da qualsiasi dispositivo: desktop, tablet e mobile.">
  <meta name="keywords" content="tende, zanzariere, tendidea, tende da sole, vendita online">
  <link rel="canonical" href="/Contenuti/IndexPROVISSIMA.HTML">
  <meta property="og:title" content="Tendidea - Catalogo tende e zanzariere">
  <meta property="og:description" content="Acquista tende e zanzariere di qualità. Spedizione e resi facili.">
  <meta property="og:type" content="website">
  <meta property="og:url" content="/Contenuti/IndexPROVISSIMA.HTML">
  <meta property="og:image" content="/Contenuti/img/xl_zanzariera.jpg">
  <script type="application/ld+json">
  { "@context": "https://schema.org",
    "@type": "Organization",
    "name": "Tendidea",
    "url": "./",
    "logo": "img/xl_zanzariera.jpg",
    "sameAs": [] }
  </script>
  <style>
    /* Responsive adjustments */
    @media (max-width: 900px) {
      .product-card { flex: 0 0 100%; height: auto; }
      .product-card img { width: 40%; }
      .product-body { width: 60%; }
      #cartSummary { width: 100%; right: -100%; }
    }

    /* show mobile menu button and hide desktop nav elements on smaller screens */
    @media (max-width: 900px) {
      .mobile-menu-btn { display:inline-flex; }
      .nav .nav-links, .auth-actions, .search-container { display: none !important; }
    }
    @media (max-width: 600px) {
      .product-card img { width: 100%; height: auto; border-radius:8px; margin-right:0; margin-bottom:8px; }
      .product-card { flex-direction: column; align-items: flex-start; padding:12px; }
      .product-body { width:100%; }
      .add-to-cart-btn { position: static; margin-top:10px; }
      /* reduce heavy background on small screens for clarity */
      body { background: #f6f8fb; background-size: auto; }
    }
    img { max-width:100%; height:auto; display:block; }
    html { scroll-behavior: smooth; }
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: url('https://wallpapers.com/images/hd/white-hd-1920-x-1080-background-9qv6jj5my4d7krx6.jpg') no-repeat center center fixed;
      background-size: cover;
      color: #222;
      overflow-x: hidden;
    }

    /* NAVBAR */
    .nav {
      background: rgba(255, 255, 255, 0.95);
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      z-index: 1000;
    }
    .nav .container-nav {
      max-width: 1200px;
      margin: auto;
      display: flex;
      justify-content: flex-start; /* logo a sinistra */
      align-items: center;
      padding: 10px 20px;
      position: relative;
      gap: 15px; /* distanza tra logo, ricerca e carrello */
    }
    /* Mobile hamburger */
    .mobile-menu-btn { display:none; background:#0074d9; color:#fff; border:none; padding:8px 10px; border-radius:8px; cursor:pointer; font-size:18px }
    .mobile-nav-overlay { display:none; position:fixed; top:56px; right:0; left:0; bottom:0; background:rgba(0,0,0,0.45); z-index:2500; align-items:flex-start; justify-content:flex-end; }
    .mobile-nav-overlay.open { display:flex; }
    .mobile-nav-inner { background:#fff; width:300px; max-width:92%; height:100%; padding:14px; box-shadow:0 8px 30px rgba(0,0,0,0.2); transform: translateX(100%); transition: transform 320ms cubic-bezier(.2,.9,.2,1); }
    .mobile-nav-overlay.open .mobile-nav-inner { transform: translateX(0); }
    .auth-actions { display:flex; gap:8px; margin-left:8px; }
    .auth-btn { padding:8px 12px; border-radius:8px; cursor:pointer; font-weight:600; border:1px solid rgba(0,0,0,0.06); }
    .auth-btn.login { background:#0074d9; color:#fff; border:none; }
    .auth-btn.register { background:transparent; color:#222; border:1px solid rgba(0,0,0,0.12); }
    .nav .logo {
      font-size: 24px;
      font-weight: bold;
      color: #0074d9;
      text-decoration: none;
      cursor: pointer;
    }
    .nav ul {
      list-style: none;
      margin: 0;
      padding: 0;
      display: flex;
      gap: 20px;
    }
    .nav ul li a {
      text-decoration: none;
      color: #222;
      font-weight: 500;
      padding: 8px 12px;
      transition: background 0.5s ease, color 0.5s ease, transform 0.3s ease;
    }
    .nav ul li a:hover {
      background: #0074d9;
      color: white;
      border-radius: 4px;
      transform: translateY(-3px);
    }

    .search-container {
      margin-left: auto; /* porta la ricerca vicino al carrello */
    }
    #searchInput {
      padding: 6px 10px;
      border-radius: 5px;
      border: 1px solid #ccc;
      font-size: 14px;
    }

    /* Icona Carrello */
    #cartIcon {
      position: relative;
      cursor: pointer;
      font-size: 24px;
      color: #0074d9;
    }

    /* Carrello a pannello scorrevole */
    #cartSummary {
      position: fixed;
      top: 0;
      right: -360px; /* nascosto inizialmente */
      width: 350px;
      height: 100%;
      background: #f9f9f9;
      padding: 25px;
      box-shadow: -6px 0 20px rgba(0,0,0,0.2);
      border-radius: 12px 0 0 12px;
      z-index: 1001;
      overflow-y: auto;
      transition: right 0.4s ease;
      font-family: Arial, sans-serif;
    }
    #cartSummary.open { right: 0; }
    #cartSummary h3 {
      margin-top: 0;
      font-weight: 600;
      color: #222;
      border-bottom: 1px solid #ddd;
      padding-bottom: 10px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    #cartSummary ul { list-style: none; padding: 0; margin: 15px 0; }
    #cartSummary ul li {
      display: flex;
      justify-content: space-between;
      margin-bottom: 10px;
      padding-bottom: 5px;
      border-bottom: 1px solid #eee;
      transition: background 0.3s;
    }
    #cartSummary ul li:hover {
      background: #eaeaea;
      border-radius: 4px;
    }
    #cartTotal {
      font-weight: bold;
      text-align: right;
      font-size: 18px;
      margin-top: 20px;
    }

    /* Feedback aggiunta al carrello */
    #cartFeedback {
      position: fixed;
      top: 50%;
      left: 50%;
      /* start slightly above center so the show animation slides into exact center */
      transform: translate(-50%, -56%);
      background: rgba(0,0,0,0.85);
      color: white;
      padding: 14px 20px;
      border-radius: 8px;
      display: none;
      z-index: 7000;
      font-size: 15px;
      box-shadow: 0 12px 40px rgba(0,0,0,0.4);
      max-width: 90%; text-align: center;
    }

    .spacer { height: 60px; }

    /* CARD PRODOTTI */
    .product-card {
      flex: 0 0 50%;
      height: 250px;
      background: #fff;
      border-radius: 10px;
      box-shadow: 0 4px 6px rgba(0,0,0,0.1);
      transition: transform 0.3s, box-shadow 0.3s;
      display: flex;
      align-items: center;
      justify-content: flex-start;
      margin-bottom: 20px;
      position: relative;
      padding: 15px;
    }
    .product-card img {
      width: 48%;
      height: auto;
      border-top-left-radius: 10px;
      border-bottom-left-radius: 10px;
      margin-right: 15px;
    }
    /* layout: two products per row horizontally occupying half screen */
    .product-grid { display:flex; flex-wrap:wrap; gap:20px; }
    .product-card .product-body { padding:12px; width:52%; }
    .product-card:hover {
      transform: translateY(-8px) scale(1.03);
      box-shadow: 0 12px 20px rgba(0,0,0,0.2);
    }

    .add-to-cart-btn {
      display: inline-block;
      padding: 10px 20px;
      background: linear-gradient(180deg,#0074d9,#005bb5);
      color: white;
      text-decoration: none;
      border-radius: 10px;
      transition: transform 220ms cubic-bezier(.2,.9,.2,1), box-shadow 220ms ease, opacity 180ms ease;
      position: absolute;
      bottom: 15px;
      right: 15px;
      margin: 0;
      box-shadow: 0 6px 14px rgba(0,123,255,0.18);
      will-change: transform;
    }
    .add-to-cart-btn:hover {
      transform: translateY(-3px) scale(1.03);
      box-shadow: 0 14px 30px rgba(0,123,255,0.16);
    }
    .add-to-cart-btn:active {
      transform: translateY(0) scale(0.98);
      opacity: 0.95;
    }

    /* Generic button styles */
    .btn {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      padding: 8px 12px;
      border-radius: 8px;
      cursor: pointer;
      border: none;
      background: #f6f6f6;
      transition: transform 160ms ease, box-shadow 160ms ease, background 160ms ease;
    }
    .btn:hover { transform: translateY(-3px); box-shadow: 0 10px 20px rgba(0,0,0,0.08); }
    .btn:active { transform: translateY(0) scale(0.99); }
    .btn-primary { background: linear-gradient(180deg,#28a745,#218838); color: #fff; box-shadow: 0 6px 16px rgba(40,167,69,0.16); }
    .pay-method { display:flex; align-items:center; gap:10px; justify-content:space-between; }
    .pay-method .method-left { display:flex; align-items:center; gap:10px; }
    .payment-logo { width:34px; height:22px; display:inline-block; }

     /* Temporaneo: nasconde caption residue dei metodi di pagamento (inline opacity:0.9)
       per evitare duplicati se è rimasto markup precedente */
     .pay-method > span[style*="opacity:0.9"] { display: none !important; }
     .pay-method .method-left + span { display: none !important; }

    /* Modal animations */
    #checkoutModal { opacity: 0; pointer-events: none; transition: opacity 260ms ease; }
    #checkoutModal.show { opacity: 1; pointer-events: auto; }
    #checkoutModal > div { transform: translateY(-8px) scale(0.98); transition: transform 260ms cubic-bezier(.2,.9,.2,1), box-shadow 260ms ease; }
    #checkoutModal.show > div { transform: translateY(0) scale(1); }

    /* Toast animation (centered) - preserve X translate and animate Y only */
    #cartFeedback { transition: opacity 260ms ease, transform 260ms cubic-bezier(.2,.9,.2,1); opacity: 0; }
    #cartFeedback.show { opacity: 1; transform: translate(-50%, -50%); }
    #cartFeedback.hide { opacity: 0; transform: translate(-50%, -56%); }
    /* Footer */
    .site-footer { background: rgba(255,255,255,0.85); border-top: 1px solid #eee; }
    .site-footer .footer-inner { max-width:1200px; margin: 16px auto; padding: 8px 20px; text-align:center; color:#666; font-size:13px; }
    /* User avatar + menu */
    .user-avatar {
      width:36px; height:36px; border-radius:50%; background:#e9eef8; color:#234c9a; border:none; display:inline-flex; align-items:center; justify-content:center; font-weight:700; cursor:pointer; box-shadow:0 2px 8px rgba(0,0,0,0.08);
    }
    .user-menu { position:absolute; right:20px; top:60px; background:#fff; border:1px solid #eee; border-radius:8px; box-shadow:0 8px 30px rgba(0,0,0,0.12); min-width:200px; overflow:hidden; z-index:3000; }
    .user-menu .menu-item { padding:10px 12px; text-align:left; border-bottom:1px solid #f3f3f3; cursor:pointer; background:transparent; width:100%; }
    .user-menu .menu-item:hover { background:#f6f9ff; }
    /* Language selector area */
    .language-area { display:flex; align-items:center; gap:8px; margin-left:12px; }
    .lang-flag-btn { width:36px; height:28px; border-radius:6px; background:#fff; border:1px solid #eee; display:inline-flex; align-items:center; justify-content:center; cursor:pointer; font-size:18px; }
    .lang-globe-btn { width:36px; height:36px; border-radius:50%; background:#f3f6fb; border:1px solid #e6eefc; display:inline-flex; align-items:center; justify-content:center; cursor:pointer; font-size:18px; }
    /* Language modal */
    #languageModal { display:none; position:fixed; inset:0; background:rgba(0,0,0,0.5); align-items:center; justify-content:center; z-index:2600; }
    #languageModal .modal-inner { background:#fff; padding:14px; border-radius:10px; width:420px; max-width:96%; box-shadow:0 12px 40px rgba(0,0,0,0.25); }
    #languageModal .lang-search { width:100%; padding:8px; border:1px solid #ddd; border-radius:6px; margin-bottom:8px; }
    #languageModal .lang-list { max-height:360px; overflow:auto; border-top:1px solid #f1f1f1; }
    #languageModal .lang-item { display:flex; gap:8px; align-items:center; padding:8px 6px; cursor:pointer; border-bottom:1px solid #fafafa; }
    #languageModal .lang-item:hover { background:#f6f9ff; }
    /* More-details panel for products */
    .more-details-btn { margin-top:8px; background:transparent; border:none; color:#0074d9; cursor:pointer; font-weight:600; display:inline-flex; align-items:center; gap:8px; }
    .product-more { overflow:hidden; max-height:0; transition: max-height 1.5s ease; font-size:13px; color:#444; margin-top:8px; }
    .product-more.open { max-height:260px; }
    .more-arrow { display:inline-block; transition: transform 300ms ease; }
    .more-arrow.open { transform: rotate(180deg); }
    /* intro overlay animation */
    #introOverlay { position:fixed; inset:0; background:#ffffff; z-index:5000; display:flex; align-items:center; justify-content:center; flex-direction:column; transform: translateY(-100%); transition: transform 1s ease, opacity 0.8s ease; }
    #introOverlay.show { transform: translateY(0%); }
    #introOverlay.hidden { transform: translateY(-100%); opacity:0; pointer-events:none; }
    #introOverlay .logo-large { font-size:28px; font-weight:700; color:#0074d9; margin-top:8px; }
  </style>
</head>
<body>

  <div id="top"></div>

  <!-- MENU -->
  <nav class="nav">
    <div class="container-nav">
      <div style="display:flex; align-items:center; gap:8px;">
        <img id="brandImg" src="https://scontent.fbri7-1.fna.fbcdn.net/v/t39.30808-6/299876829_584062196604180_7692658332015285145_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=6ee11a&_nc_ohc=C28QtqxSBQ0Q7kNvwHPVjsg&_nc_oc=AdlbogF4yalPoL9v93AffRPjVEMkgygRVTwZ2ZbuBrsEFZ8WAOCGo59Iw0p3A3luQFM&_nc_zt=23&_nc_ht=scontent.fbri7-1.fna&_nc_gid=BneWSvETip7O4-1tqn7hqw&oh=00_Afi50R0KveiNPFj090YvD6HcygOJRb8DG7a-RZdYtzKyzQ&oe=692A0AF9" alt="brand" style="width:36px;height:36px;border-radius:6px;object-fit:cover;">
        <a href="#top" class="logo">Tendidea</a>
      </div>
      <div class="nav-links" style="display:flex; gap:10px; margin-left:12px;">
        <button id="aboutBtn" class="btn">Chi siamo</button>
        <button id="returnsRefundBtn" class="btn">Resi e rimborsi</button>
      </div>
      <div class="auth-actions">
        <button id="loginBtn" class="auth-btn login">Accedi</button>
        <button id="registerBtn" class="auth-btn register">Registrati</button>
      </div>

      <!-- Icona Carrello -->
      <div id="cartIcon">🛒</div>

      <!-- Barra di ricerca accanto al carrello -->
      <div class="search-container">
        <input type="text" id="searchInput" placeholder="Cerca prodotto...">
      </div>
      <!-- Language selector: flag + globe -->
      <div class="language-area" id="languageArea">
        <button id="selectedFlagBtn" class="lang-flag-btn" title="Lingua selezionata">🇮🇹</button>
        <button id="openLangBtn" class="lang-globe-btn" title="Seleziona lingua">🌐</button>
        <button id="mobileMenuBtn" class="mobile-menu-btn" title="Menu">☰</button>
      </div>
    </div>
  </nav>

  <!-- Mobile navigation overlay -->
  <div id="mobileNavOverlay" class="mobile-nav-overlay" aria-hidden="true">
    <div class="mobile-nav-inner">
      <div style="display:flex; align-items:center; justify-content:space-between; margin-bottom:8px;">
        <div style="font-weight:700; font-size:18px; color:#0074d9">Tendidea</div>
        <button id="closeMobileNav" class="btn" style="background:#f1f1f1;">✖</button>
      </div>
      <div style="display:flex; flex-direction:column; gap:8px;">
        <button id="m_aboutBtn" class="btn">Chi siamo</button>
        <button id="m_returnsRefundBtn" class="btn">Resi e rimborsi</button>
        <button id="m_loginBtn" class="btn btn-primary">Accedi</button>
        <button id="m_registerBtn" class="btn">Registrati</button>
      </div>
    </div>
  </div>

  <!-- Feedback aggiunta -->
  <div id="cartFeedback">Prodotto aggiunto al carrello!</div>

  <!-- Pannello carrello -->
  <div id="cartSummary">
    <h3>
      Carrello
      <button id="closeCart" style="cursor:pointer; background:none; border:none; font-size:18px;">✖</button>
    </h3>
    <ul id="cartItems"></ul>
    <div id="cartTotal">Totale: 0,00 €</div>
    <div style="margin-top:12px; text-align:right;">
      <button id="checkoutBtn" style="padding:8px 12px; background:#28a745; color:white; border:none; border-radius:6px; cursor:pointer;">Check Out</button>
    </div>
  </div>

  <!-- Modal Checkout (nascosto) -->
  <div id="checkoutModal" style="display:none; position:fixed; inset:0; background:rgba(0,0,0,0.5); align-items:center; justify-content:center; z-index:2002;">
    <div style="background:#fff; padding:18px; border-radius:10px; width:420px; max-width:94%; box-shadow:0 8px 30px rgba(0,0,0,0.3);">
      <h3 style="margin:0 0 10px 0;">Scegli il metodo di pagamento</h3>
      <!-- Shipping form: first step of checkout -->
      <div id="shippingForm" style="display:none; flex-direction:column; gap:8px; margin-bottom:10px;">
        <h4 style="margin:0 0 6px 0;">Indirizzo di spedizione</h4>
        <label style="font-size:13px">Paese</label>
        <select id="shipCountry" style="width:100%; padding:8px; border-radius:6px; border:1px solid #ddd; margin-bottom:6px;"></select>
        <label style="font-size:13px">Città</label>
        <input id="shipCity" type="text" style="width:100%; padding:8px; border-radius:6px; border:1px solid #ddd; margin-bottom:6px;">
        <label style="font-size:13px">Provincia / Stato</label>
        <input id="shipProvince" type="text" style="width:100%; padding:8px; border-radius:6px; border:1px solid #ddd; margin-bottom:6px;">
        <label style="font-size:13px">Indirizzo</label>
        <input id="shipAddress" type="text" style="width:100%; padding:8px; border-radius:6px; border:1px solid #ddd; margin-bottom:6px;">
        <div style="display:flex; justify-content:flex-end; gap:8px;">
          <button id="cancelShipping" class="btn" style="background:#f1f1f1;">Annulla</button>
          <button id="proceedShipping" class="btn btn-primary">Procedi al pagamento</button>
        </div>
      </div>

      <div id="paymentMethods" style="display:flex; flex-direction:column; gap:10px;">
        <button class="pay-method pay-option" data-method="paypal" style="background:#003087; color:#fff; height:56px; display:flex; align-items:center; gap:12px; padding:10px 14px; border-radius:8px; border:none; font-weight:600;">
          <span class="payment-logo"><svg viewBox="0 0 64 32" xmlns="http://www.w3.org/2000/svg" width="34" height="22"><rect width="64" height="32" rx="4" fill="#003087"/><path d="M18 22c2-5 7-9 13-9 6 0 11 3 13 7 0 0 2-10-2-14-4-4-12-5-20-3-8 2-13 7-14 13-1 6 2 11 6 10z" fill="#009CDE"/></svg></span>
          <span>PayPal</span>
        </button>

        <button class="pay-method pay-option" data-method="mybank" style="background:linear-gradient(90deg,#0ea5a4,#7c3aed); color:#fff; height:56px; display:flex; align-items:center; gap:12px; padding:10px 14px; border-radius:8px; border:none; font-weight:600;">
          <span class="payment-logo"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="34" height="22"><path d="M12 2L2 7h20L12 2zM4 9v11h5V9H4zm6 0v11h4V9h-4zm6 0v11h4V9h-4z" fill="#fff"/></svg></span>
          <span>MyBank</span>
        </button>

        <button class="pay-method pay-option" data-method="card" style="background:linear-gradient(90deg,#3b82f6,#1e3a8a); color:#fff; height:56px; display:flex; align-items:center; gap:12px; padding:10px 14px; border-radius:8px; border:none; font-weight:600;">
          <span class="payment-logo"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 16" width="34" height="22"><rect width="24" height="16" rx="2" fill="#fff" opacity="0.14"/><rect x="2" y="3" width="20" height="3" fill="#fff" opacity="0.9"/></svg></span>
          <span>Carta di credito / debito</span>
        </button>

        <div id="paypalFlow" style="display:none; margin-top:8px;">
          <div id="paypal-button-container"></div>
        </div>
      </div>

      <!-- Card form (hidden by default) -->
      <div id="cardForm" style="display:none; margin-top:12px;">
        <label style="display:block; font-size:13px; margin-bottom:6px;">Intestatario</label>
        <input id="cardName" type="text" placeholder="Nome e Cognome" style="width:100%; padding:8px; margin-bottom:8px; border-radius:6px; border:1px solid #ddd;">
        <label style="display:block; font-size:13px; margin-bottom:6px;">Numero carta</label>
        <input id="cardNumber" type="text" inputmode="numeric" placeholder="0000 0000 0000 0000" maxlength="23" style="width:100%; padding:8px; margin-bottom:8px; border-radius:6px; border:1px solid #ddd;">
        <div style="display:flex; gap:8px;">
          <div style="flex:1;">
            <label style="display:block; font-size:13px; margin-bottom:6px;">Scadenza (MM/AA)</label>
            <input id="cardExp" type="text" placeholder="MM/AA" maxlength="5" style="width:100%; padding:8px; border-radius:6px; border:1px solid #ddd;">
          </div>
          <div style="width:110px;">
            <label style="display:block; font-size:13px; margin-bottom:6px;">CVC</label>
            <input id="cardCvc" type="text" inputmode="numeric" maxlength="4" placeholder="CVC" style="width:100%; padding:8px; border-radius:6px; border:1px solid #ddd;">
          </div>
        </div>
        <div style="display:flex; justify-content:flex-end; gap:8px; margin-top:12px;">
          <button id="cancelCard" class="btn" style="background:#f1f1f1;">Indietro</button>
          <button id="submitCard" class="btn btn-primary">Paga</button>
        </div>
      </div>

      <!-- Bank transfer instructions -->
      <div id="bankForm" style="display:none; margin-top:12px; font-size:14px; color:#333;">
        <p style="margin:0 0 8px 0;">Bonifico bancario - istruzioni</p>
        <div style="background:#fafafa; padding:10px; border-radius:6px; border:1px solid #eee;">
          <div style="margin-bottom:6px;"><strong>Beneficiario:</strong> Tende & Zanzariere</div>
          <div style="margin-bottom:6px;"><strong>Indirizzo:</strong> Via Dante 39, 70016 Noicattaro (BA)</div>
          <div style="margin-bottom:6px;"><strong>IBAN:</strong> <span id="ibanText">IT00 XXXX XXXX XXXX XXXX XXXX XXX</span> <button id="copyIban" class="btn" style="padding:4px 6px; font-size:12px;">Copia</button></div>
          <div style="margin-bottom:6px;"><strong>Causale:</strong> Pagamento ordine - inserire riferimento cliente/ordine</div>
        </div>
        <div style="display:flex; justify-content:flex-end; gap:8px; margin-top:12px;">
          <button id="cancelBank" class="btn" style="background:#f1f1f1;">Indietro</button>
          <button id="confirmBank" class="btn btn-primary">Ho effettuato bonifico</button>
        </div>
      </div>

      <div id="modalFooter" style="display:flex; justify-content:flex-end; gap:8px; margin-top:12px;">
        <button id="cancelCheckout" class="btn" style="background:#f1f1f1;">Annulla</button>
      </div>
    </div>
  </div>

  <!-- Login Modal -->
  <div id="loginModal" style="display:none; position:fixed; inset:0; background:rgba(0,0,0,0.5); align-items:center; justify-content:center; z-index:2100;">
    <div style="background:#fff; padding:18px; border-radius:10px; width:360px; max-width:94%; box-shadow:0 8px 30px rgba(0,0,0,0.3);">
      <h3 style="margin:0 0 10px 0;">Accedi</h3>
      <label style="font-size:13px">Email</label>
      <input id="loginEmail" type="email" style="width:100%; padding:8px; margin-bottom:8px; border-radius:6px; border:1px solid #ddd;">
      <label style="font-size:13px">Password</label>
      <div style="display:flex; gap:6px; align-items:center;">
        <input id="loginPassword" type="password" style="flex:1; padding:8px; margin-bottom:8px; border-radius:6px; border:1px solid #ddd;">
        <button id="toggleLoginPwd" class="btn" title="Mostra/Nascondi password" style="padding:6px; margin-bottom:8px;">👁️</button>
      </div>
      <div style="display:flex; gap:8px; justify-content:space-between; align-items:center; margin-top:8px;">
        <button id="doLogin" class="btn btn-primary">Accedi</button>
        <button id="googleLogin" class="btn google-btn" style="background:#fff; padding:8px 12px; font-weight:700; display:flex; align-items:center; gap:8px;">
          <img src="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 533.5 544.3'><path fill='%23EA4335' d='M533.5 278.4c0-18.5-1.5-37-4.6-54.8H272v103.8h147.3c-6.4 34.6-25.7 63.9-54.7 83.4l88.2 68c51.6-47.5 81.7-118 81.7-200.4z'/><path fill='%234285F4' d='M272 544.3c73.9 0 136-24.5 181.3-66.7l-88.2-68c-24.5 16.4-55.8 26-93.1 26-71.6 0-132.3-48.3-154.1-113.4L24.7 354.2C70.1 452.6 165 544.3 272 544.3z'/><path fill='%23FBBC05' d='M117.9 325.9c-9.7-28.8-9.7-59.9 0-88.7L24.7 177.6C-9 258.5-9 345.8 24.7 426.6l93.2-100.7z'/><path fill='%2327A757' d='M272 107.1c39.9 0 75.8 13.7 104 40.6l77.8-77.8C410.2 24.3 344.7 0 272 0 165 0 70.1 91.7 24.7 190.1l93.2 100.7C139.7 155.4 200.4 107.1 272 107.1z'/></svg>" alt="G" style="width:18px;height:18px;">
          <span style="font-size:15px;">Accedi con Google</span>
        </button>
        <button id="closeLogin" class="btn" style="background:#f1f1f1">Annulla</button>
      </div>
      <div id="loginMsg" style="color:red; margin-top:8px; display:none;"></div>
      <div style="margin-top:8px; font-size:13px; color:#333;">
        Non hai un account? <button id="toRegisterFromLogin" class="auth-btn register" style="padding:6px 10px; font-size:13px;">Registrati</button>
      </div>
    </div>
  </div>

  <!-- Register Modal -->
  <div id="registerModal" style="display:none; position:fixed; inset:0; background:rgba(0,0,0,0.5); align-items:center; justify-content:center; z-index:2100;">
    <div style="background:#fff; padding:18px; border-radius:10px; width:380px; max-width:94%; box-shadow:0 8px 30px rgba(0,0,0,0.3);">
      <h3 style="margin:0 0 10px 0;">Registrati</h3>
      <label style="display:block; font-size:13px; margin-bottom:6px;">Nome</label>
      <input id="regName" type="text" placeholder="Nome" style="width:100%; padding:8px; margin-bottom:8px; border-radius:6px; border:1px solid #ddd;">
      <label style="display:block; font-size:13px; margin-bottom:6px;">Cognome</label>
      <input id="regSurname" type="text" placeholder="Cognome" style="width:100%; padding:8px; margin-bottom:8px; border-radius:6px; border:1px solid #ddd;">
      <label style="font-size:13px">Email</label>
      <input id="regEmail" type="email" style="width:100%; padding:8px; margin-bottom:8px; border-radius:6px; border:1px solid #ddd;">
      <label style="font-size:13px">Password</label>
      <div style="display:flex; gap:6px; align-items:center;">
        <input id="regPassword" type="password" style="flex:1; padding:8px; margin-bottom:8px; border-radius:6px; border:1px solid #ddd;">
        <button id="toggleRegPwd" class="btn" title="Mostra/Nascondi password" style="padding:6px; margin-bottom:8px;">👁️</button>
      </div>
      <label style="font-size:13px">Conferma Password</label>
      <div style="display:flex; gap:6px; align-items:center;">
        <input id="regPassword2" type="password" style="flex:1; padding:8px; margin-bottom:8px; border-radius:6px; border:1px solid #ddd;">
        <button id="toggleRegPwd2" class="btn" title="Mostra/Nascondi password" style="padding:6px; margin-bottom:8px;">👁️</button>
      </div>
      <div style="display:flex; gap:8px; justify-content:flex-end; margin-top:8px;">
        <button id="doRegister" class="btn btn-primary">Registrati</button>
        <button id="closeRegister" class="btn" style="background:#f1f1f1">Annulla</button>
      </div>
      <div id="regMsg" style="color:red; margin-top:8px; display:none;"></div>
      <div style="margin-top:8px; font-size:13px; color:#333;">
        Hai già fatto l'accesso? <button id="toLoginFromRegister" class="auth-btn login" style="padding:6px 10px; font-size:13px;">Accedi</button>
      </div>
    </div>
  </div>

  <!-- Product Detail Modal -->
  <div id="productDetailModal" style="display:none; position:fixed; inset:0; background:rgba(0,0,0,0.6); align-items:center; justify-content:center; z-index:2150;">
    <div style="background:#fff; padding:18px; border-radius:10px; width:900px; max-width:96%; box-shadow:0 8px 40px rgba(0,0,0,0.4); display:flex; gap:16px;">
      <div style="flex:1; max-width:420px;">
        <img id="detailImg" src="" style="width:100%; height:auto; border-radius:8px; object-fit:cover;">
        <div style="display:flex; gap:8px; margin-top:8px;" id="detailThumbs"></div>
      </div>
      <div style="flex:1;">
        <h2 id="detailTitle">Titolo prodotto</h2>
        <p id="detailPrice">Prezzo</p>
        <p id="detailDesc">Descrizione breve del prodotto.</p>
        <div style="display:flex; gap:8px; margin-top:12px;">
          <button id="detailAddToCart" class="btn btn-primary">Aggiungi al carrello</button>
          <button id="detailClose" class="btn">Chiudi</button>
        </div>
      </div>
    </div>
  </div>

  <!-- Verify Code Modal -->
  <div id="verifyModal" style="display:none; position:fixed; inset:0; background:rgba(0,0,0,0.6); align-items:center; justify-content:center; z-index:2200;">
    <div style="background:#fff; padding:18px; border-radius:10px; width:420px; max-width:94%; box-shadow:0 8px 30px rgba(0,0,0,0.3); text-align:center;">
      <h3 style="margin:0 0 10px 0;">Verifica email</h3>
      <p style="margin:0 0 12px 0;">Controlla la tua casella postale: ti abbiamo inviato un codice a 6 cifre.</p>
      <div id="verifyCodeHint" style="margin:0 0 8px 0; color:#444; font-size:13px; text-align:center;"></div>
      <div id="verifyInputs" style="display:flex; gap:8px; justify-content:center; margin-bottom:12px;"></div>
      <div style="display:flex; gap:8px; justify-content:center;"
        <button id="doVerify" class="btn btn-primary">Verifica</button>
        <button id="resendCode" class="btn">Rinvia codice</button>
        <button id="closeVerify" class="btn" style="background:#f1f1f1">Annulla</button>
      </div>
      <div id="verifyMsg" style="color:red; margin-top:8px; display:none;"></div>
    </div>
  </div>

  <div class="spacer"></div>

    <!-- Logout Confirmation Modal -->
    <div id="logoutConfirmModal" style="display:none; position:fixed; inset:0; background:rgba(0,0,0,0.5); align-items:center; justify-content:center; z-index:2300;">
      <div style="background:#fff; padding:18px; border-radius:10px; width:360px; max-width:94%; box-shadow:0 8px 30px rgba(0,0,0,0.3); text-align:center;">
        <h3 style="margin:0 0 10px 0;">Sei sicuro di voler uscire?</h3>
        <p style="margin:0 0 16px 0; color:#444;">Verrai disconnesso dal tuo account.</p>
        <div style="display:flex; gap:10px; justify-content:center;">
          <button id="confirmLogoutNo" class="btn" style="background:#f1f1f1;">No</button>
          <button id="confirmLogoutYes" class="btn btn-primary">Sì, esci</button>
        </div>
      </div>
    </div>

  <!-- CONTENUTO PRODOTTI -->
  <div style="max-width: 1200px; margin: auto; padding: 20px;">
    <div class="product-grid">
      <div class="product-card" data-name="bora libera installazione" data-price="59.90" data-desc="Zanzariera pratica per porte e finestre." data-images="img/xl_zanzariera.jpg,img/xl_zanzariera.jpg">
        <img src="img/xl_zanzariera.jpg" alt="Zanzariera Bora">
        <div class="product-body">
          <h3>Bora (libera installazione)</h3>
          <p>Prezzo: 59,90 €</p>
          <a href="#" class="add-to-cart-btn">Aggiungi al carrello</a>
        </div>
      </div>
      <div class="product-card" data-name="bora rullo laterale" data-price="69.90" data-desc="Rullo laterale di alta qualità." data-images="img/xl_zanzariera.jpg,img/xl_zanzariera.jpg">
        <img src="img/xl_zanzariera.jpg" alt="Bora Rullo Laterale">
        <div class="product-body">
          <h3>Bora Rullo Laterale</h3>
          <p>Prezzo: 69,90 €</p>
          <a href="#" class="add-to-cart-btn">Aggiungi al carrello</a>
        </div>
      </div>
      <div class="product-card" data-name="bora avvolgibile" data-price="79.90" data-desc="Avvolgibile per finestre e balconi." data-images="img/xl_zanzariera.jpg,img/xl_zanzariera.jpg">
        <img src="img/xl_zanzariera.jpg" alt="Bora Avvolgibile">
        <div class="product-body">
          <h3>Bora Avvolgibile</h3>
          <p>Prezzo: 79,90 €</p>
          <a href="#" class="add-to-cart-btn">Aggiungi al carrello</a>
        </div>
      </div>
      <div class="product-card" data-name="modello verticale" data-price="49.00" data-desc="Modello verticale, semplice e robusto." data-images="img/xl_zanzariera.jpg,img/xl_zanzariera.jpg">
        <img src="img/xl_zanzariera.jpg" alt="Zanzariera Verticale">
        <div class="product-body">
          <h3>Modello Verticale</h3>
          <p>Prezzo: 49,00 €</p>
          <a href="#" class="add-to-cart-btn">Aggiungi al carrello</a>
        </div>
      </div>
      <div class="product-card" data-name="pannello scorrevole" data-price="79.90" data-desc="Pannello scorrevole elegante." data-images="img/xl_zanzariera.jpg,img/xl_zanzariera.jpg">
        <img src="img/xl_zanzariera.jpg" alt="Pannello Scorrevole">
        <div class="product-body">
          <h3>Pannello Scorrevole</h3>
          <p>Prezzo: 79,90 €</p>
          <a href="#" class="add-to-cart-btn">Aggiungi al carrello</a>
        </div>
      </div>
      <div class="product-card" data-name="xl zanzariera" data-price="99.90" data-desc="XL Zanzariera per grandi aperture." data-images="img/xl_zanzariera.jpg,img/xl_zanzariera.jpg">
        <img src="img/xl_zanzariera.jpg" alt="Zanzariera XL">
        <div class="product-body">
          <h3>XL Zanzariera</h3>
          <p>Prezzo: 99,90 €</p>
          <a href="#" class="add-to-cart-btn">Aggiungi al carrello</a>
        </div>
      </div>
    </div>
  </div>

  <!-- Language selection modal -->
  <div id="languageModal">
    <div class="modal-inner">
      <h3 style="margin:0 0 8px 0;">Seleziona lingua</h3>
      <input id="langSearch" class="lang-search" placeholder="Cerca lingua (es. Italiano, English, العربية)...">
      <div class="lang-list" id="langList"></div>
      <div style="display:flex; justify-content:flex-end; margin-top:8px;"><button id="closeLangModal" class="btn" style="background:#f1f1f1">Chiudi</button></div>
    </div>
  </div>
<script>
  // Fallback PayPal client id fornito dall'utente per test rapido
  // ATTENZIONE: questa è una modifica temporanea per test in sandbox.
  const FALLBACK_PAYPAL_CLIENT_ID = 'ATeLYkFQ65bzxoiGFDvOlgNpC_Mmq-Gzq9bzMBYI1ekvLs-5OZzY-njp_DZKn8uD7TsLwzEJprE1fvrt';
  // small helper to add listeners safely and log missing elements
  function addListener(elOrId, evt, handler) {
    try {
      const el = (typeof elOrId === 'string') ? document.getElementById(elOrId) : elOrId;
      if (!el) { console.warn('addListener: missing element', elOrId); return; }
      el.addEventListener(evt, handler);
    } catch (e) { console.warn('addListener error for', elOrId, e); }
  }
  // Ricerca prodotti
  document.getElementById("searchInput").addEventListener("input", function() {
    const query = this.value.toLowerCase();
    document.querySelectorAll(".product-card").forEach(card => {
      const name = card.dataset.name.toLowerCase();
      card.style.display = name.includes(query) ? "flex" : "none";
    });
  });

  const cartIcon = document.getElementById('cartIcon');
  const cartSummary = document.getElementById('cartSummary');

  function parsePrice(text) {
    if (typeof text === 'number') return text;
    if (!text) return 0;
    let t = String(text).replace(/[€\s]/g, '');
    t = t.replace(/\./g, '').replace(',', '.');
    const n = parseFloat(t);
    return isNaN(n) ? 0 : n;
  }

  function getCart() {
    try {
      const raw = localStorage.getItem('carrello');
      if (!raw) return [];
      const parsed = JSON.parse(raw);
      if (!Array.isArray(parsed)) return [];
      return parsed.map(i => ({
        name: String(i.name || ''),
        price: parsePrice(i.price),
        quantity: Number(i.quantity) || 1
      }));
    } catch (e) { return []; }
  }

  function saveCart(cart) {
    localStorage.setItem('carrello', JSON.stringify(cart));
  }

  function updateCartSummary() {
    const cart = getCart();
    const cartItems = document.getElementById('cartItems');
    const cartTotal = document.getElementById('cartTotal');
    cartItems.innerHTML = '';
    let total = 0;

    cart.forEach((item, index) => {
      total += (item.price || 0) * (item.quantity || 1);

      const li = document.createElement('li');
      li.style.display = 'flex';
      li.style.justifyContent = 'space-between';
      li.style.alignItems = 'center';

      const left = document.createElement('div');
      left.style.display = 'flex';
      left.style.flexDirection = 'column';
      left.textContent = item.name;

      const right = document.createElement('div');
      right.style.display = 'flex';
      right.style.alignItems = 'center';
      right.style.gap = '8px';

      const qty = document.createElement('small');
      qty.textContent = 'x' + (item.quantity || 1);
      right.appendChild(qty);

      const priceSpan = document.createElement('span');
      priceSpan.textContent = ((item.price * (item.quantity || 1)).toFixed(2)).replace('.', ',') + ' €';
      right.appendChild(priceSpan);

      const removeBtn = document.createElement('button');
      removeBtn.textContent = '✖';
      removeBtn.style.background = 'none';
      removeBtn.style.border = 'none';
      removeBtn.style.cursor = 'pointer';
      removeBtn.addEventListener('click', () => {
        const c = getCart();
        c.splice(index, 1);
        saveCart(c);
        updateCartSummary();
      });
      right.appendChild(removeBtn);

      li.appendChild(left);
      li.appendChild(right);
      cartItems.appendChild(li);
    });

    cartTotal.textContent = (getTranslation('cartTotalPrefix')||'Totale: ') + formatCurrency(total);

    let cartCount = document.getElementById('cartCount');
    if(!cartCount) {
      cartCount = document.createElement('span');
      cartCount.id = 'cartCount';
      cartCount.style.position = 'absolute';
      cartCount.style.top = '-8px';
      cartCount.style.right = '-8px';
      cartCount.style.background = 'red';
      cartCount.style.color = 'white';
      cartCount.style.fontSize = '12px';
      cartCount.style.padding = '2px 6px';
      cartCount.style.borderRadius = '50%';
      cartIcon.appendChild(cartCount);
    }
    cartCount.textContent = getCart().reduce((acc, i) => acc + (i.quantity || 1), 0);
  }

  function toggleCart(open = null) {
    if(open === true) cartSummary.classList.add('open');
    else if(open === false) cartSummary.classList.remove('open');
    else cartSummary.classList.toggle('open');
    updateCartSummary();
  }

  cartIcon.addEventListener('click', () => toggleCart());
  document.getElementById('closeCart').addEventListener('click', () => toggleCart(false));

  // Checkout: mostra modal con metodi di pagamento
  const checkoutBtn = document.getElementById('checkoutBtn');
  const checkoutModal = document.getElementById('checkoutModal');
  const cancelCheckout = document.getElementById('cancelCheckout');

  

  // Gestione scelta metodo di pagamento (form carta + simulazioni)
  const paymentMethodButtons = document.querySelectorAll('.pay-method');
  const paymentMethodsDiv = document.getElementById('paymentMethods');
  const cardFormDiv = document.getElementById('cardForm');
  const cancelCard = document.getElementById('cancelCard');
  const submitCard = document.getElementById('submitCard');

  function showToast(text, timeout = 2200) {
    const feedback = document.getElementById('cartFeedback');
    if (!feedback) return;
    feedback.textContent = text;
    feedback.style.display = 'block';
    feedback.classList.add('show');
    // ensure centered visual; remove after timeout
    clearTimeout(feedback._hideTimeout);
    feedback._hideTimeout = setTimeout(() => {
      feedback.classList.remove('show');
      feedback.style.display = 'none';
    }, timeout);
  }

  function openCheckout() {
    const cart = getCart();
    if (!cart || cart.length === 0) {
      showToast('Il carrello è vuoto.', 1500);
      return;
    }
    // reset views: show shipping form first
    const shippingForm = document.getElementById('shippingForm');
    if (shippingForm) {
      paymentMethodsDiv.style.display = 'none';
      cardFormDiv.style.display = 'none';
      shippingForm.style.display = 'flex';
      // populate countries select
      populateCountrySelect();
    } else {
      paymentMethodsDiv.style.display = 'flex';
      cardFormDiv.style.display = 'none';
    }
    // assicurati che eventuali flow rimasti siano nascosti
    const pf = document.getElementById('paypalFlow'); if (pf) pf.style.display = 'none';
    const bf = document.getElementById('bankForm'); if (bf) bf.style.display = 'none';
    checkoutModal.classList.add('show');
    checkoutModal.style.display = 'flex';
  }

  function closeCheckout() {
    checkoutModal.classList.remove('show');
    checkoutModal.style.display = 'none';
    // nascondi e resetta tutti i sotto-pannelli per evitare duplicati al riaprire
    const pf = document.getElementById('paypalFlow'); if (pf) { pf.style.display = 'none'; }
    const bf = document.getElementById('bankForm'); if (bf) { bf.style.display = 'none'; }
    if (cardFormDiv) cardFormDiv.style.display = 'none';
    // pulisci container PayPal (se presente) per evitare render doppi in casi strani
    const pcont = document.getElementById('paypal-button-container'); if (pcont) pcont.innerHTML = '';
  }

  paymentMethodButtons.forEach(btn => {
    btn.addEventListener('click', () => {
      const method = btn.dataset.method;
      // If shipping form is visible, do not allow payment selection until shipping completed
      const shippingForm = document.getElementById('shippingForm');
      if (shippingForm && shippingForm.style.display !== 'none') { showToast('Compila prima le informazioni di spedizione',2200); return; }
      if (method === 'card') {
        // mostra il form carta
        paymentMethodsDiv.style.display = 'none';
        cardFormDiv.style.display = 'block';
        document.getElementById('cardName').focus();
        return;
      }

      if (method === 'paypal') {
        // mostra area PayPal e renderizza i bottoni SDK
        paymentMethodsDiv.style.display = 'none';
        cardFormDiv.style.display = 'none';
        document.getElementById('paypalFlow').style.display = 'block';
        // carica SDK dinamicamente: USIAMO IL FALLBACK interno e non tentiamo la fetch a /config
        (function(){
          const clientId = FALLBACK_PAYPAL_CLIENT_ID || '';
          if (!clientId) { showToast('PayPal non configurato e nessun fallback disponibile.'); paymentMethodsDiv.style.display = 'flex'; document.getElementById('paypalFlow').style.display = 'none'; return; }
          showToast('Carico PayPal SDK...');
          if (!window.paypal) {
            const script = document.createElement('script');
            const currency = localStorage.getItem('selectedCurrency') || 'EUR';
            script.src = 'https://www.paypal.com/sdk/js?client-id=' + encodeURIComponent(clientId) + '&currency=' + encodeURIComponent(currency);
            script.onload = () => renderPayPalButtons();
            script.onerror = () => { showToast('Impossibile caricare PayPal SDK'); paymentMethodsDiv.style.display = 'flex'; document.getElementById('paypalFlow').style.display = 'none'; };
            document.head.appendChild(script);
          } else {
            renderPayPalButtons();
          }
        })();
        return;
      }
      if (method === 'bank' || method === 'mybank') {
        // mostra le istruzioni per bonifico / MyBank
        paymentMethodsDiv.style.display = 'none';
        cardFormDiv.style.display = 'none';
        document.getElementById('bankForm').style.display = 'block';
        return;
      }

      // Altri metodi: simulazione generica
      const cart = getCart();
      const total = cart.reduce((s, it) => s + ((Number(it.price) || 0) * (Number(it.quantity) || 1)), 0);
      closeCheckout();
      showToast(`Pagamento (${method}) eseguito: ${total.toFixed(2).replace('.', ',')} €`, 2600);
      saveCart([]);
      updateCartSummary();
    });
  });

  // Render PayPal Buttons - usa server-side endpoints per creare/catturare ordine
  function renderPayPalButtons() {
    try {
      if (!window.paypal) return;
      // evita doppio render
      if (document.querySelector('#paypal-button-container').children.length) return;

      // Prefer server-side order creation/capture if available
      window.paypal.Buttons({
        createOrder: function(data, actions) {
          const cart = getCart();
          const total = cart.reduce((s, it) => s + ((Number(it.price) || 0) * (Number(it.quantity) || 1)), 0).toFixed(2);
          // try server create-order
          return fetch('/create-order', { method: 'post', headers: { 'Content-Type': 'application/json' }, body: JSON.stringify({ amount: total }) })
            .then(res => res.json())
            .then(json => {
              if (json && json.id) return json.id;
              // fallback to client-side create
              const currency = localStorage.getItem('selectedCurrency') || 'EUR';
              return actions.order.create({ purchase_units: [{ amount: { currency_code: currency, value: String(total) } }] });
            }).catch(()=>{
              const currency = localStorage.getItem('selectedCurrency') || 'EUR';
              return actions.order.create({ purchase_units: [{ amount: { currency_code: currency, value: String(total) } }] });
            });
        },
        onApprove: function(data, actions) {
          // try server capture first
          if (data && data.orderID) {
            return fetch('/capture-order', { method: 'post', headers: { 'Content-Type': 'application/json' }, body: JSON.stringify({ orderId: data.orderID }) })
              .then(res => res.json())
              .then(json => {
                closeCheckout(); saveCart([]); updateCartSummary(); showToast('Pagamento PayPal riuscito (server)', 2600);
              }).catch(()=>{
                return actions.order.capture().then(function(details){ closeCheckout(); showToast('Pagamento PayPal riuscito', 2600); saveCart([]); updateCartSummary(); }).catch(function(e){ showToast('Errore nella cattura PayPal'); });
              });
          }
          // fallback to client capture
          return actions.order.capture().then(function(details){ closeCheckout(); showToast('Pagamento PayPal riuscito', 2600); saveCart([]); updateCartSummary(); }).catch(function(err){ showToast('Errore nella cattura PayPal'); });
        },
        onError: function(err) { console.error('PayPal error', err); showToast('Errore PayPal, riprova', 2600); }
      }).render('#paypal-button-container');
    } catch (e) { console.error(e); }
  }

  // annulla il form carta (torna ai metodi)
  cancelCard.addEventListener('click', (e) => {
    e.preventDefault();
    cardFormDiv.style.display = 'none';
    paymentMethodsDiv.style.display = 'flex';
  });

  // bank form buttons
  const cancelBank = document.getElementById('cancelBank');
  const confirmBank = document.getElementById('confirmBank');
  const copyIbanBtn = document.getElementById('copyIban');
  const ibanText = document.getElementById('ibanText');
  cancelBank.addEventListener('click', (e) => {
    e.preventDefault();
    document.getElementById('bankForm').style.display = 'none';
    paymentMethodsDiv.style.display = 'flex';
  });
  confirmBank.addEventListener('click', async (e) => {
    e.preventDefault();
    // invia una conferma di bonifico al server per registrare la richiesta
    const cart = getCart();
    const total = cart.reduce((s, it) => s + ((Number(it.price) || 0) * (Number(it.quantity) || 1)), 0).toFixed(2);
    const reference = 'REF-' + Date.now();
    const payload = { orderId: null, reference, amount: total };

    confirmBank.disabled = true;
    confirmBank.textContent = 'Invio...';
    try {
      // if a local test server is intentionally used (set localStorage 'useLocalServer'='true'), try to call it
      const useLocal = localStorage.getItem('useLocalServer') === 'true';
      if (useLocal) {
        const res = await fetch('http://localhost:3000/confirm-bank', {
          method: 'post', headers: { 'Content-Type': 'application/json' }, body: JSON.stringify(payload)
        });
        const data = await res.json();
        if (res.ok) {
          const pending = { id: data.order && data.order.id ? data.order.id : reference, reference, amount: total, status: data.order && data.order.status ? data.order.status : 'pending_bank' };
          localStorage.setItem('bankPending', JSON.stringify(pending));
          showToast('Conferma bonifico inviata. Attendi verifica amministrativa.', 4200);
          document.getElementById('bankForm').style.display = 'none';
          closeCheckout();
        } else {
          showToast('Errore invio conferma bonifico', 3600);
        }
      } else {
        // fallback offline: registra localmente la richiesta senza contattare server
        const pending = { id: reference, reference, amount: total, status: 'pending_bank_offline' };
        localStorage.setItem('bankPending', JSON.stringify(pending));
        showToast('Conferma bonifico registrata (modalità offline). Attendi verifica.', 4200);
        document.getElementById('bankForm').style.display = 'none';
        closeCheckout();
      }
    } catch (err) {
      // If anything goes wrong, fallback to local registration to avoid noisy console network errors
      const pending = { id: reference, reference, amount: total, status: 'pending_bank_offline' };
      localStorage.setItem('bankPending', JSON.stringify(pending));
      showToast('Registrazione conferma bonifico locale (errore rete).', 4200);
    } finally {
      confirmBank.disabled = false;
      confirmBank.textContent = 'Ho effettuato bonifico';
    }
  });
  copyIbanBtn.addEventListener('click', (e) => {
    const text = ibanText.textContent || '';
    navigator.clipboard && navigator.clipboard.writeText(text).then(() => {
      showToast('IBAN copiato negli appunti');
    }).catch(() => { showToast('Copia non supportata'); });
  });

  // Shipping form handlers
  const cancelShippingBtn = document.getElementById('cancelShipping');
  const proceedShippingBtn = document.getElementById('proceedShipping');
  if (cancelShippingBtn) cancelShippingBtn.addEventListener('click', ()=>{ document.getElementById('shippingForm').style.display='none'; closeCheckout(); });
  if (proceedShippingBtn) proceedShippingBtn.addEventListener('click', (e)=>{
    e.preventDefault();
    const country = document.getElementById('shipCountry')?.value || '';
    const city = document.getElementById('shipCity')?.value.trim() || '';
    const province = document.getElementById('shipProvince')?.value.trim() || '';
    const address = document.getElementById('shipAddress')?.value.trim() || '';
    // stronger validation: basic heuristics
    const isAlpha = (s) => /[A-Za-zÀ-ÖØ-öø-ÿ\s'-]+$/.test(s);
    if (!country || !city || !address) { showToast('Compila Paese, Città e Indirizzo', 2200); return; }
    if (!isAlpha(city) || city.length < 2) { showToast('Credenziali errate: città non valida', 2600); return; }
    if (province && province.length < 2) { showToast('Credenziali errate: provincia non valida', 2600); return; }
    if (address.length < 5) { showToast('Credenziali errate: indirizzo non valido', 2600); return; }
    const shipping = { country, city, province, address };
    localStorage.setItem('checkoutShipping', JSON.stringify(shipping));
    // hide shipping, show payment methods
    document.getElementById('shippingForm').style.display='none';
    paymentMethodsDiv.style.display = 'flex';
    // ensure PayPal flow reset
    const pf = document.getElementById('paypalFlow'); if (pf) pf.style.display = 'none';
  });

  // --- Country / currency helpers ---
  function populateCountrySelect(){
    const sel = document.getElementById('shipCountry'); if (!sel) return;
    const countries = [
      { code:'IT', name:'Italia', currency:'EUR', flag:'🇮🇹' },
      { code:'DE', name:'Germania', currency:'EUR', flag:'🇩🇪' },
      { code:'FR', name:'Francia', currency:'EUR', flag:'🇫🇷' },
      { code:'ES', name:'Spagna', currency:'EUR', flag:'🇪🇸' },
      { code:'GB', name:'Regno Unito', currency:'GBP', flag:'🇬🇧' },
      { code:'US', name:'United States', currency:'USD', flag:'🇺🇸' },
      { code:'CN', name:'China', currency:'CNY', flag:'🇨🇳' }
    ];
    sel.innerHTML = '';
    const stored = localStorage.getItem('selectedCountry') || 'IT';
    countries.forEach(c=>{ const opt = document.createElement('option'); opt.value = c.code; opt.textContent = c.name + ' (' + c.code + ')'; opt.dataset.currency = c.currency; opt.dataset.flag = c.flag; if (c.code === stored) opt.selected = true; sel.appendChild(opt); });
    sel.addEventListener('change', ()=>{
      const chosen = sel.options[sel.selectedIndex];
      const cur = chosen.dataset.currency || 'EUR';
      localStorage.setItem('selectedCountry', chosen.value);
      localStorage.setItem('selectedCurrency', cur);
      // update displayed flag in navbar if desired (do not change language)
      const flag = chosen.dataset.flag || '🏳️';
      const selectedFlagBtn = document.getElementById('selectedFlagBtn'); if (selectedFlagBtn) selectedFlagBtn.textContent = flag;
      applyTranslations(); renderPrices();
    });
  }

  function renderPrices(){
    // update product card prices
    document.querySelectorAll('.product-card').forEach(card=>{
      const p = card.dataset.price || '0';
      const el = card.querySelector('.product-body p');
      if (el) el.textContent = formatCurrency(Number(p));
    });
    // update detail price if open
    const dp = document.getElementById('detailPrice'); if (dp && dp.textContent){
      // detailPrice is set when opening product; rely on open detail handler to set proper format
    }
    updateCartSummary();
  }


  // formattazione campo numero carta (gruppi di 4)
  const cardNumberInput = document.getElementById('cardNumber');
  cardNumberInput.addEventListener('input', (e) => {
    const v = e.target.value.replace(/\D/g, '').slice(0,19);
    const parts = [];
    for (let i=0;i<v.length;i+=4) parts.push(v.substr(i,4));
    e.target.value = parts.join(' ');
  });

  // formattazione expiry MM/AA
  const cardExpInput = document.getElementById('cardExp');
  cardExpInput.addEventListener('input', (e) => {
    const v = e.target.value.replace(/\D/g, '').slice(0,4);
    if (v.length >= 3) e.target.value = v.slice(0,2) + '/' + v.slice(2);
    else e.target.value = v;
  });

  // submit form carta (simulazione di pagamento)
  submitCard.addEventListener('click', (e) => {
    e.preventDefault();
    const name = document.getElementById('cardName').value.trim();
    const number = cardNumberInput.value.replace(/\s/g,'');
    const exp = cardExpInput.value.trim();
    const cvc = document.getElementById('cardCvc').value.trim();

    // validazioni semplici
    if (!name) { showToast('Inserisci nome titolare'); return; }
    if (!/^[0-9]{13,19}$/.test(number)) { showToast('Numero carta non valido'); return; }
    if (!/^(0[1-9]|1[0-2])\/[0-9]{2}$/.test(exp)) { showToast('Scadenza non valida (MM/AA)'); return; }
    if (!/^[0-9]{3,4}$/.test(cvc)) { showToast('CVC non valido'); return; }

    // simulazione process
    const cart = getCart();
    const total = cart.reduce((s, it) => s + ((Number(it.price) || 0) * (Number(it.quantity) || 1)), 0);
    // show processing
    submitCard.textContent = 'Elaborazione...';
    submitCard.disabled = true;
    setTimeout(() => {
      submitCard.textContent = 'Paga';
      submitCard.disabled = false;
      closeCheckout();
      showToast(`Pagamento con carta eseguito: ${total.toFixed(2).replace('.', ',')} €`, 2800);
      saveCart([]);
      updateCartSummary();
      // pulizia campi
      document.getElementById('cardName').value = '';
      cardNumberInput.value = '';
      cardExpInput.value = '';
      document.getElementById('cardCvc').value = '';
    }, 1200);
  });

  // collega i pulsanti del modal alle funzioni di apertura/chiusura
  checkoutBtn.addEventListener('click', openCheckout);
  cancelCheckout.addEventListener('click', closeCheckout);

  document.querySelectorAll('.add-to-cart-btn').forEach(btn => {
    btn.addEventListener('click', e => {
      e.preventDefault();
      const currentUser = localStorage.getItem('currentUser');
      const card = btn.closest('.product-card');
      const title = card.dataset.name || card.querySelector('h3').textContent || '';
      const priceNum = Number(card.dataset.price) || (function(){ const t = card.querySelector('p').textContent; const m = t.match(/[\d,.]+/); return m?parsePrice(m[0]):0; })();
      if (!currentUser) {
        // require login: save pending add and open login modal
        localStorage.setItem('pendingAdd', JSON.stringify({ name: title, price: priceNum }));
        loginModal.style.display = 'flex';
        showToast('Devi effettuare l\'accesso per aggiungere al carrello', 2200);
        return;
      }
      const cart = getCart();
      const found = cart.find(i => i.name === title);
      if (found) found.quantity = (found.quantity || 1) + 1; else cart.push({ name: title, price: priceNum, quantity: 1 });
      saveCart(cart);
      toggleCart(true);
      showToast('Aggiunto al carrello', 1500);
    });
  });

  // Scroll lento 1,5s logo
  document.querySelector('.logo').addEventListener('click', function(e) {
    e.preventDefault();
    const start = window.scrollY;
    const duration = 1500;
    let startTime = null;

    function scrollStep(timestamp) {
      if (!startTime) startTime = timestamp;
      const progress = timestamp - startTime;
      const percent = Math.min(progress / duration, 1);
      window.scrollTo(0, start * (1 - percent));
      if (progress < duration) requestAnimationFrame(scrollStep);
    }
    requestAnimationFrame(scrollStep);
  });

  updateCartSummary();

  // --- AUTH (client-side, localStorage users) ---
  const loginBtnEl = document.getElementById('loginBtn');
  const registerBtnEl = document.getElementById('registerBtn');
  const loginModal = document.getElementById('loginModal');
  const registerModal = document.getElementById('registerModal');
  const closeLogin = document.getElementById('closeLogin');
  const closeRegister = document.getElementById('closeRegister');
  const doLogin = document.getElementById('doLogin');
  const doRegister = document.getElementById('doRegister');
  const googleLogin = document.getElementById('googleLogin');
  const loginMsg = document.getElementById('loginMsg');
  const regMsg = document.getElementById('regMsg');

  function getUsers() { try { return JSON.parse(localStorage.getItem('users')||'[]'); } catch(e){return [];} }
  function saveUsers(u){ localStorage.setItem('users', JSON.stringify(u)); }
  function findUserByEmail(email){ return getUsers().find(x=>x.email && x.email.toLowerCase()===email.toLowerCase()); }
  function setCurrentUser(u){
    let userObj = u || {};
    try {
      if (userObj.email) {
        const found = findUserByEmail(userObj.email);
        if (found) {
          // merge stored profile fields (name, surname, etc.) but avoid persisting password
          const { password, verifyCode, ...rest } = found;
          userObj = Object.assign({}, rest, userObj);
        }
      }
    } catch(e){}
    localStorage.setItem('currentUser', JSON.stringify(userObj));
    renderUserArea();
  }

  // --- Currency / formatting and i18n ---
  function formatCurrency(amount){
    const currency = localStorage.getItem('selectedCurrency') || 'EUR';
    try {
      const n = Number(amount) || 0;
      return new Intl.NumberFormat(localStorage.getItem('selectedLanguage') || 'it-IT', { style:'currency', currency }).format(n);
    } catch(e) { return (Number(amount)||0).toFixed(2) + ' ' + (currency==='EUR'? '€' : currency); }
  }

  // Simple translations map (extendable)
  var TRANSLATIONS = {
    it: {
      login: 'Accedi', register: 'Registrati', cart: 'Carrello', cartTotalPrefix: 'Totale: ', choosePayment: 'Scegli il metodo di pagamento', shippingTitle: 'Indirizzo di spedizione', proceedShipping: 'Procedi al pagamento', about: 'Chi siamo', returns: 'Reso', refund: 'Rimborso', moreDetails: 'Più dettagli', lessDetails: 'Chiudi dettagli'
    },
    en: {
      login: 'Sign in', register: 'Register', cart: 'Cart', cartTotalPrefix: 'Total: ', choosePayment: 'Choose payment method', shippingTitle: 'Shipping address', proceedShipping: 'Proceed to payment', about: 'About us', returns: 'Returns', refund: 'Refund', moreDetails: 'More details', lessDetails: 'Hide details'
    }
  };

  function getTranslation(key){
    try {
      const lang = (localStorage.getItem('selectedLanguage') || 'it').slice(0,2);
      const map = (typeof TRANSLATIONS === 'object' && TRANSLATIONS) ? TRANSLATIONS : {};
      return (map[lang] && map[lang][key]) || null;
    } catch (e) {
      console.warn('getTranslation fallback', e);
      return null;
    }
  }

  function applyTranslations(){
    // Buttons
    const ln = (localStorage.getItem('selectedLanguage')||'it').slice(0,2);
    document.getElementById('loginBtn').textContent = getTranslation('login') || 'Accedi';
    document.getElementById('registerBtn').textContent = getTranslation('register') || 'Registrati';
    document.getElementById('checkoutBtn').textContent = getTranslation('choosePayment') || document.getElementById('checkoutBtn').textContent;
    // new nav buttons
    const aboutEl = document.getElementById('aboutBtn'); if (aboutEl) aboutEl.textContent = getTranslation('about') || 'Chi siamo';
    const returnsRefundEl = document.getElementById('returnsRefundBtn'); if (returnsRefundEl) returnsRefundEl.textContent = 'Resi e rimborsi';
    // more-details buttons on product cards
    document.querySelectorAll('.more-details-btn .more-text').forEach(node=>{ node.textContent = getTranslation('moreDetails') || 'Più dettagli'; });
    // cart total updated by updateCartSummary
    updateCartSummary();
  }

  // initialize language setting if missing
  if (!localStorage.getItem('selectedLanguage')) localStorage.setItem('selectedLanguage','it');
  if (!localStorage.getItem('selectedCurrency')) localStorage.setItem('selectedCurrency','EUR');
  applyTranslations();

  loginBtnEl.addEventListener('click', ()=>{ loginModal.style.display='flex'; });
  registerBtnEl.addEventListener('click', ()=>{ registerModal.style.display='flex'; });
  closeLogin.addEventListener('click', ()=>{ loginModal.style.display='none'; loginMsg.style.display='none'; });
  closeRegister.addEventListener('click', ()=>{ registerModal.style.display='none'; regMsg.style.display='none'; });

  // Password show/hide toggles
  const toggleLoginPwd = document.getElementById('toggleLoginPwd');
  const toggleRegPwd = document.getElementById('toggleRegPwd');
  const toggleRegPwd2 = document.getElementById('toggleRegPwd2');
  if (toggleLoginPwd) toggleLoginPwd.addEventListener('click', ()=>{ const inp = document.getElementById('loginPassword'); if (!inp) return; inp.type = inp.type === 'password' ? 'text' : 'password'; toggleLoginPwd.textContent = inp.type === 'password' ? '👁️' : '🙈'; });
  if (toggleRegPwd) toggleRegPwd.addEventListener('click', ()=>{ const inp = document.getElementById('regPassword'); if (!inp) return; inp.type = inp.type === 'password' ? 'text' : 'password'; toggleRegPwd.textContent = inp.type === 'password' ? '👁️' : '🙈'; });
  if (toggleRegPwd2) toggleRegPwd2.addEventListener('click', ()=>{ const inp = document.getElementById('regPassword2'); if (!inp) return; inp.type = inp.type === 'password' ? 'text' : 'password'; toggleRegPwd2.textContent = inp.type === 'password' ? '👁️' : '🙈'; });

  doRegister.addEventListener('click', (e)=>{
    e.preventDefault();
    const name = document.getElementById('regName').value.trim();
    const surname = document.getElementById('regSurname').value.trim();
    const email = document.getElementById('regEmail').value.trim();
    const p1 = document.getElementById('regPassword').value;
    const p2 = document.getElementById('regPassword2').value;
    if (!name || !surname) { regMsg.textContent='Nome e cognome richiesti'; regMsg.style.display='block'; return; }
    if (!email || !p1) { regMsg.textContent='Email e password richieste'; regMsg.style.display='block'; return; }
    if (p1 !== p2) { regMsg.textContent='Le password non coincidono'; regMsg.style.display='block'; return; }
    if (findUserByEmail(email)) { regMsg.textContent='Account già registrato'; regMsg.style.display='block'; return; }
    // create user with verification code and prompt for verification
    const code = String(Math.floor(100000 + Math.random()*900000));
    const users = getUsers(); users.push({ name, surname, email, password: p1, createdAt: Date.now(), verified: false, verifyCode: code }); saveUsers(users);
    // store which email is being verified
    localStorage.setItem('verifyingEmail', email);
    regMsg.style.display='none'; registerModal.style.display='none';
    console.log('Verification code for', email, ':', code);
    showToast('Registrazione avvenuta. Controlla la tua casella postale per il codice.', 4000);
    // open verify modal
    openVerifyModal();
  });

  doLogin.addEventListener('click', (e)=>{
    e.preventDefault();
    const email = document.getElementById('loginEmail').value.trim();
    const pwd = document.getElementById('loginPassword').value;
    const u = findUserByEmail(email);
    if (!u) { loginMsg.textContent='Account non trovato, registrati'; loginMsg.style.display='block'; return; }
    if (u.password !== pwd) { loginMsg.textContent='Password errata'; loginMsg.style.display='block'; return; }
    if (!u.verified) {
      // prompt verification
      localStorage.setItem('verifyingEmail', email);
      loginModal.style.display='none';
      showToast('Account non verificato. Controlla la tua casella postale.', 3000);
      openVerifyModal();
      return;
    }
    setCurrentUser({ email }); loginMsg.style.display='none'; loginModal.style.display='none'; showToast('Accesso effettuato', 2200);
    // if pending add exists, add to cart
    const pending = localStorage.getItem('pendingAdd');
    if (pending) {
      try {
        const p = JSON.parse(pending);
        const cart = getCart(); const found = cart.find(i=>i.name===p.name);
        if (found) found.quantity = (found.quantity||1)+1; else cart.push({ name: p.name, price: Number(p.price)||0, quantity: 1 });
        saveCart(cart); updateCartSummary(); toggleCart(true);
      } catch(e){}
      localStorage.removeItem('pendingAdd');
    }
  });

  // listen for a message from the google popup (our controlled popup will postMessage when user confirms)
  window.addEventListener('message', function onGoogleMsg(ev){
    try {
      if (!ev.data || ev.data !== 'google-signed') return;
      // create or reuse simulated google user and login
      const email = 'google-simulated@example.com';
      let u = findUserByEmail(email);
      if (!u) { const users = getUsers(); users.push({ name:'Google', surname:'User', email, password: null, oauth: 'google', createdAt: Date.now() }); saveUsers(users); }
      setCurrentUser({ email }); loginModal.style.display='none'; showToast('Accesso con Google effettuato',2200);
      window.removeEventListener('message', onGoogleMsg);
    } catch(e){}
  });

  googleLogin.addEventListener('click', ()=>{
    // open a small controlled popup that writes its HTML via document.write (avoids complex template literals)
    const popup = window.open('', 'google_popup', 'width=520,height=480');
    if (!popup) { showToast('Impossibile aprire popup. Consenti popup nel browser.', 3500); return; }
    const html = [
      '<!doctype html><html><head><meta charset="utf-8"><title>Login Google</title>',
      '<style>body{font-family:Arial,sans-serif;padding:18px;} .btn{display:inline-block;padding:8px 12px;border-radius:6px;background:#1a73e8;color:#fff;border:none;cursor:pointer;margin:6px 0;} .link{display:block;margin:8px 0;color:#1a73e8;cursor:pointer;text-decoration:underline;}</style>',
      '</head><body>',
      '<h3>Accesso Google</h3>',
      '<p>Si aprirà la pagina ufficiale di Google in una nuova finestra; effettua l\'accesso e poi torna qui e premi "Ho effettuato l\'accesso" per completare il login.</p>',
      '<button id="openBtn" class="btn">Apri schermata login Google</button>',
      '<div><button id="confirmBtn" class="btn" style="background:#28a745;">Ho effettuato l\'accesso</button></div>',
      '<p style="margin-top:10px;font-size:13px;color:#666">Se vuoi forzare l\'inserimento delle credenziali, seleziona "Usa un altro account" nella schermata Google.</p>',
      '<script>document.getElementById("openBtn").addEventListener("click",function(){window.open("https://accounts.google.com/ServiceLogin?continue=https://www.google.com/","_blank");});',
      'document.getElementById("confirmBtn").addEventListener("click",function(){try{window.opener.postMessage("google-signed","*");}catch(e){}window.close();});<\/script>',
      '</body></html>'
    ].join('');
    try {
      popup.document.open();
      popup.document.write(html);
      popup.document.close();
    } catch (e) {
      // If writing to popup is blocked, provide instruction
      showToast('Popup bloccato o non scrivibile. Consenti popup nel browser.', 3800);
    }
  });

  // modal switching buttons
  const toLoginFromRegister = document.getElementById('toLoginFromRegister');
  const toRegisterFromLogin = document.getElementById('toRegisterFromLogin');
  if (toLoginFromRegister) toLoginFromRegister.addEventListener('click', ()=>{ registerModal.style.display='none'; loginModal.style.display='flex'; });
  if (toRegisterFromLogin) toRegisterFromLogin.addEventListener('click', ()=>{ loginModal.style.display='none'; registerModal.style.display='flex'; });

  // Render user avatar/menu or show auth actions
  function renderUserArea(){
    const authActions = document.querySelector('.auth-actions');
    const existing = document.getElementById('userArea'); if (existing) existing.remove();
    const cu = localStorage.getItem('currentUser');
    // Always show avatar; when logged out menu offers Accedi/Registrati, when logged in shows profile + Esci
    try {
      const user = cu ? JSON.parse(cu) : {};
      if (authActions) authActions.style.display = cu ? 'none' : 'none'; // we keep auth actions hidden when avatar exists
      const ua = document.createElement('div'); ua.id = 'userArea'; ua.style.position='relative'; ua.style.display='flex'; ua.style.alignItems='center'; ua.style.gap='8px';
      const avatarBtn = document.createElement('button'); avatarBtn.id = 'userAvatarBtn'; avatarBtn.className = 'user-avatar';
      const initials = ((user.name||'') + ' ' + (user.surname||'') || (user.email||'' ) ).split(' ').map(s=>s? s[0].toUpperCase():'').join('').slice(0,2) || 'U';
      avatarBtn.textContent = initials; avatarBtn.title = user.email || 'Account';
      ua.appendChild(avatarBtn);
      const menu = document.createElement('div'); menu.id = 'userMenu'; menu.className='user-menu'; menu.style.display='none';
      if (cu) {
        const displayName = ((user.name||'') + (user.surname? ' '+user.surname : '')) || user.email || '';
        menu.innerHTML = '<div style="padding:10px 12px; font-weight:700; border-bottom:1px solid #f5f5f5;">'+(displayName||'Utente')+'<div style="font-size:13px; color:#666; font-weight:400;">'+(user.email||'')+'</div></div>' +
          '<button id="userSettings" class="menu-item">Impostazioni</button>' +
          '<button id="userLogout" class="menu-item">Esci</button>';
      } else {
        menu.innerHTML = '<div style="padding:10px 12px; font-weight:700; border-bottom:1px solid #f5f5f5;">Account<div style="font-size:13px; color:#666; font-weight:400;">Non sei connesso</div></div>' +
          '<button id="menuLogin" class="menu-item">Accedi</button>' +
          '<button id="menuRegister" class="menu-item">Registrati</button>';
      }
      ua.appendChild(menu);
      document.querySelector('.container-nav').appendChild(ua);

      avatarBtn.addEventListener('click', (e)=>{ e.stopPropagation(); menu.style.display = menu.style.display==='block' ? 'none' : 'block'; });
      if (cu) {
        document.getElementById('userLogout').addEventListener('click', ()=>{ menu.style.display='none'; document.getElementById('logoutConfirmModal').style.display='flex'; });
      } else {
        document.getElementById('menuLogin').addEventListener('click', ()=>{ menu.style.display='none'; loginModal.style.display='flex'; });
        document.getElementById('menuRegister').addEventListener('click', ()=>{ menu.style.display='none'; registerModal.style.display='flex'; });
      }
      // hide menu on outside click
      document.addEventListener('click', (ev)=>{ const uaEl = document.getElementById('userArea'); if (uaEl && !uaEl.contains(ev.target)) { const m = document.getElementById('userMenu'); if (m) m.style.display='none'; } });
    } catch(e){ if (authActions) authActions.style.display='flex'; }
  }
  // initial render
  renderUserArea();

  // --- Product detail modal handlers ---
  const productCards = document.querySelectorAll('.product-card');
  const productDetailModal = document.getElementById('productDetailModal');
  const detailImg = document.getElementById('detailImg');
  const detailTitle = document.getElementById('detailTitle');
  const detailPrice = document.getElementById('detailPrice');
  const detailDesc = document.getElementById('detailDesc');
  const detailThumbs = document.getElementById('detailThumbs');
  const detailAddToCart = document.getElementById('detailAddToCart');
  const detailClose = document.getElementById('detailClose');

  productCards.forEach(card=>{
    card.style.cursor='pointer';
    card.addEventListener('click', (e)=>{
      // avoid click on add-to-cart inside card
      if (e.target && (e.target.classList && e.target.classList.contains('add-to-cart-btn'))) return;
      const title = card.dataset.name || card.querySelector('h3')?.textContent || '';
      const price = card.dataset.price || '0.00';
      const desc = card.dataset.desc || card.querySelector('p')?.textContent || '';
      const imgs = (card.dataset.images || '').split(',').map(s=>s.trim()).filter(Boolean);
      detailTitle.textContent = title;
      detailPrice.textContent = 'Prezzo: ' + (Number(price).toFixed(2)).replace('.',',') + ' €';
      detailDesc.textContent = desc;
      if (imgs.length) { detailImg.src = imgs[0]; }
      detailThumbs.innerHTML = '';
      imgs.forEach(src=>{
        const im = document.createElement('img'); im.src = src; im.style.width='80px'; im.style.height='50px'; im.style.objectFit='cover'; im.style.cursor='pointer'; im.style.borderRadius='4px'; im.style.border='1px solid #ddd'; im.addEventListener('click', ()=> detailImg.src = src); detailThumbs.appendChild(im);
      });
      productDetailModal.style.display='flex';
      // add to cart handler
      detailAddToCart.onclick = (ev)=>{
        ev.preventDefault();
        const currentUser = localStorage.getItem('currentUser');
        const name = title; const priceNum = Number(price) || 0;
        if (!currentUser) {
          localStorage.setItem('pendingAdd', JSON.stringify({ name, price: priceNum }));
          productDetailModal.style.display='none';
          loginModal.style.display='flex';
          showToast('Effettua l\'accesso per aggiungere al carrello',2200);
          return;
        }
        const cart = getCart(); const found = cart.find(i=>i.name===name);
        if (found) found.quantity = (found.quantity||1)+1; else cart.push({ name, price: priceNum, quantity: 1 }); saveCart(cart); updateCartSummary(); showToast('Aggiunto al carrello',1600);
      };
    });
  });
  // ensure detail price uses selected currency
  productCards.forEach(card=>{ const price = Number(card.dataset.price||0); const pEl = card.querySelector('.product-body p'); if (pEl) pEl.textContent = formatCurrency(price); });
  detailClose.addEventListener('click', ()=>{ productDetailModal.style.display='none'; });

  // Add 'Più dettagli' toggle panels to product cards (animated 1.5s)
  productCards.forEach(card=>{
    try {
      const body = card.querySelector('.product-body');
      if (!body) return;
      // create button if missing
      if (!body.querySelector('.more-details-btn')){
        const btn = document.createElement('button'); btn.className = 'more-details-btn'; btn.type='button'; btn.innerHTML = '<span class="more-text">' + (getTranslation('moreDetails') || 'Più dettagli') + '</span> <span class="more-arrow">▾</span>';
        body.appendChild(btn);
        const more = document.createElement('div'); more.className = 'product-more'; more.innerHTML = '<strong>Informazioni:</strong> ' + (card.dataset.desc || 'Dettagli prodotto');
        body.appendChild(more);
        btn.addEventListener('click', (e)=>{ e.preventDefault(); const arrow = btn.querySelector('.more-arrow'); const txt = btn.querySelector('.more-text'); const open = more.classList.toggle('open'); if (arrow) arrow.classList.toggle('open', open); if (txt) txt.textContent = open ? (getTranslation('lessDetails')||'Chiudi dettagli') : (getTranslation('moreDetails')||'Più dettagli'); });
      }
    } catch(e){ console.warn('more-details attach failed', e); }
  });

  // --- Verify modal logic ---
  const verifyModal = document.getElementById('verifyModal');
  const verifyInputsDiv = document.getElementById('verifyInputs');
  const doVerifyBtn = document.getElementById('doVerify');
  const resendCodeBtn = document.getElementById('resendCode');
  const closeVerifyBtn = document.getElementById('closeVerify');
  const verifyMsg = document.getElementById('verifyMsg');

  function openVerifyModal(){
    // build 6 input boxes
    verifyInputsDiv.innerHTML = '';
    for (let i=0;i<6;i++){
      const inp = document.createElement('input'); inp.type='text'; inp.maxLength=1; inp.style.width='40px'; inp.style.height='40px'; inp.style.textAlign='center'; inp.style.background='#f1f1f1'; inp.style.border='1px solid #ddd'; inp.style.borderRadius='6px'; inp.style.fontSize='18px'; inp.dataset.idx = i;
      inp.addEventListener('input', (e)=>{ if (e.target.value.length) { const next = verifyInputsDiv.querySelector('input[data-idx="'+(Number(e.target.dataset.idx)+1)+'"]'); if (next) next.focus(); } });
      inp.addEventListener('keydown', (e)=>{ if (e.key === 'Backspace' && !e.target.value){ const prev = verifyInputsDiv.querySelector('input[data-idx="'+(Number(e.target.dataset.idx)-1)+'"]'); if (prev) prev.focus(); } });
      verifyInputsDiv.appendChild(inp);
    }
    verifyMsg.style.display='none';
    // show simulated code (if available) to help testing
    const verifying = localStorage.getItem('verifyingEmail');
    const hintElId = 'verifyCodeHint';
    let hintEl = document.getElementById(hintElId);
    if (!hintEl) {
      hintEl = document.createElement('div'); hintEl.id = hintElId; hintEl.style.marginTop = '8px'; hintEl.style.fontSize = '13px'; hintEl.style.color = '#444'; hintEl.style.textAlign = 'center';
      verifyModal.querySelector('.modal-inner') || verifyModal.appendChild(hintEl);
    }
    if (verifying) {
      const u = findUserByEmail(verifying);
      if (u && u.verifyCode) hintEl.textContent = 'Codice (simulazione): ' + u.verifyCode; else hintEl.textContent = '';
    } else { hintEl.textContent = ''; }
    verifyModal.style.display='flex';
  }

  async function sendVerificationCode(email){
    // in our simulated flow the code is stored on user.verifyCode; we 'resend' by regenerating
    const users = getUsers(); const uidx = users.findIndex(x=>x.email && x.email.toLowerCase()===email.toLowerCase());
    if (uidx === -1) return false;
    const code = String(Math.floor(100000 + Math.random()*900000));
    users[uidx].verifyCode = code; users[uidx].verified = false; saveUsers(users);
    console.log('Resent verification code for', email, ':', code);
    return true;
  }

  doVerifyBtn.addEventListener('click', (e)=>{
    e.preventDefault();
    const email = localStorage.getItem('verifyingEmail');
    if (!email) { verifyMsg.textContent='Nessuna email da verificare'; verifyMsg.style.display='block'; return; }
    const inputs = Array.from(verifyInputsDiv.querySelectorAll('input')).map(i=>i.value||'').join('');
    if (inputs.length !== 6) { verifyMsg.textContent='Inserisci il codice completo'; verifyMsg.style.display='block'; return; }
    const u = findUserByEmail(email);
    if (!u) { verifyMsg.textContent='Account non trovato'; verifyMsg.style.display='block'; return; }
    if (u.verifyCode === inputs) {
      // verified
      const users = getUsers(); const idx = users.findIndex(x=>x.email && x.email.toLowerCase()===email.toLowerCase()); if (idx!==-1){ users[idx].verified = true; delete users[idx].verifyCode; saveUsers(users); }
      setCurrentUser({ email }); verifyModal.style.display='none'; localStorage.removeItem('verifyingEmail'); showToast('Email verificata. Accesso effettuato.', 3000);
      // handle pending add
      const pending = localStorage.getItem('pendingAdd');
      if (pending) { try{ const p = JSON.parse(pending); const cart = getCart(); const found = cart.find(i=>i.name===p.name); if (found) found.quantity = (found.quantity||1)+1; else cart.push({ name: p.name, price: Number(p.price)||0, quantity: 1 }); saveCart(cart); updateCartSummary(); toggleCart(true); }catch(e){} localStorage.removeItem('pendingAdd'); }
    } else {
      verifyMsg.textContent='Codice non corretto'; verifyMsg.style.display='block';
    }
  });

  resendCodeBtn.addEventListener('click', async ()=>{
    const email = localStorage.getItem('verifyingEmail'); if (!email) return;
    await sendVerificationCode(email);
    // update visible hint if modal open
    const u = findUserByEmail(email);
    const hint = document.getElementById('verifyCodeHint'); if (hint) hint.textContent = u && u.verifyCode ? ('Codice (simulazione): ' + u.verifyCode) : '';
    showToast('Codice rinviato. Controlla la tua casella postale.', 2500);
  });

  closeVerifyBtn.addEventListener('click', ()=>{ verifyModal.style.display='none'; });

  // Logout confirmation modal handlers
  const confirmLogoutYes = document.getElementById('confirmLogoutYes');
  const confirmLogoutNo = document.getElementById('confirmLogoutNo');
  if (confirmLogoutNo) confirmLogoutNo.addEventListener('click', ()=>{ document.getElementById('logoutConfirmModal').style.display='none'; });
  if (confirmLogoutYes) confirmLogoutYes.addEventListener('click', ()=>{
    // clear current user and re-render UI
    localStorage.removeItem('currentUser');
    document.getElementById('logoutConfirmModal').style.display='none';
    renderUserArea();
    showToast('Logout effettuato',2000);
    // open login modal after logout
    loginModal.style.display='flex';
  });

  // --- Language selector logic ---
  const languageModal = document.getElementById('languageModal');
  const openLangBtn = document.getElementById('openLangBtn');
  const closeLangModal = document.getElementById('closeLangModal');
  const langListEl = document.getElementById('langList');
  const langSearch = document.getElementById('langSearch');
  const selectedFlagBtn = document.getElementById('selectedFlagBtn');

  const languages = [
    { code:'it', name:'Italiano', native:'Italiano', flag:'🇮🇹' },
    { code:'en', name:'English', native:'English', flag:'🇺🇸' },
    { code:'es', name:'Español', native:'Español', flag:'🇪🇸' },
    { code:'fr', name:'Français', native:'Français', flag:'🇫🇷' },
    { code:'de', name:'Deutsch', native:'Deutsch', flag:'🇩🇪' },
    { code:'ru', name:'Русский', native:'Русский', flag:'🇷🇺' },
    { code:'zh', name:'中文', native:'中文', flag:'🇨🇳' },
    { code:'ja', name:'日本語', native:'日本語', flag:'🇯🇵' },
    { code:'ko', name:'한국어', native:'한국어', flag:'🇰🇷' },
    { code:'ar', name:'العربية', native:'العربية', flag:'🇸🇦' },
    { code:'hi', name:'हिन्दी', native:'हिन्दी', flag:'🇮🇳' },
    { code:'bn', name:'বাংলা', native:'বাংলা', flag:'🇧🇩' },
    { code:'ur', name:'اردو', native:'اردو', flag:'🇵🇰' },
    { code:'tr', name:'Türkçe', native:'Türkçe', flag:'🇹🇷' },
    { code:'pl', name:'Polski', native:'Polski', flag:'🇵🇱' },
    { code:'nl', name:'Nederlands', native:'Nederlands', flag:'🇳🇱' },
    { code:'el', name:'Ελληνικά', native:'Ελληνικά', flag:'🇬🇷' },
    { code:'sv', name:'Svenska', native:'Svenska', flag:'🇸🇪' },
    { code:'no', name:'Norsk', native:'Norsk', flag:'🇳🇴' },
    { code:'da', name:'Dansk', native:'Dansk', flag:'🇩🇰' },
    { code:'fi', name:'Suomi', native:'Suomi', flag:'🇫🇮' },
    { code:'hu', name:'Magyar', native:'Magyar', flag:'🇭🇺' },
    { code:'cs', name:'Čeština', native:'Čeština', flag:'🇨🇿' },
    { code:'sk', name:'Slovenčina', native:'Slovenčina', flag:'🇸🇰' },
    { code:'hr', name:'Hrvatski', native:'Hrvatski', flag:'🇭🇷' },
    { code:'sr', name:'Српски', native:'Српски', flag:'🇷🇸' },
    { code:'ro', name:'Română', native:'Română', flag:'🇷🇴' },
    { code:'bg', name:'Български', native:'Български', flag:'🇧🇬' },
    { code:'lt', name:'Lietuvių', native:'Lietuvių', flag:'🇱🇹' },
    { code:'lv', name:'Latviešu', native:'Latviešu', flag:'🇱🇻' },
    { code:'et', name:'Eesti', native:'Eesti', flag:'🇪🇪' },
    { code:'he', name:'עברית', native:'עברית', flag:'🇮🇱' },
    { code:'th', name:'ไทย', native:'ไทย', flag:'🇹🇭' },
    { code:'vi', name:'Tiếng Việt', native:'Tiếng Việt', flag:'🇻🇳' },
    { code:'tl', name:'Filipino', native:'Filipino', flag:'🇵🇭' },
    { code:'ms', name:'Bahasa Melayu', native:'Bahasa Melayu', flag:'🇲🇾' },
    { code:'id', name:'Bahasa Indonesia', native:'Bahasa Indonesia', flag:'🇮🇩' },
    { code:'af', name:'Afrikaans', native:'Afrikaans', flag:'🇿🇦' },
    { code:'sw', name:'Kiswahili', native:'Kiswahili', flag:'🇰🇪' },
    { code:'fa', name:'فارسی', native:'فارسی', flag:'🇮🇷' },
    { code:'ca', name:'Català', native:'Català', flag:'🇪🇸' },
    { code:'ga', name:'Gaeilge', native:'Gaeilge', flag:'🇮🇪' },
    { code:'cy', name:'Cymraeg', native:'Cymraeg', flag:'🏴'},
    { code:'sq', name:'Shqip', native:'Shqip', flag:'🇦🇱' },
    { code:'mk', name:'Македонски', native:'Македонски', flag:'🇲🇰' },
    { code:'hy', name:'Հայերեն', native:'Հայերեն', flag:'🇦🇲' },
    { code:'az', name:'Azərbaycan', native:'Azərbaycan', flag:'🇦🇿' },
    { code:'kk', name:'Қазақша', native:'Қазақша', flag:'🇰🇿' },
    { code:'uz', name:'Oʻzbekcha', native:'Oʻzbekcha', flag:'🇺🇿' },
    { code:'bn-IN', name:'Bangla (India)', native:'বাংলা', flag:'🇮🇳' }
  ];

  function renderLangList(filter=''){
    langListEl.innerHTML = '';
    const f = filter.trim().toLowerCase();
    languages.forEach(l=>{
      if (f && !(l.name.toLowerCase().includes(f) || (l.native||'').toLowerCase().includes(f) || l.code.toLowerCase().includes(f))) return;
      const it = document.createElement('div'); it.className='lang-item'; it.innerHTML = '<div style="width:36px; text-align:center">'+(l.flag||'🏳️')+'</div><div style="flex:1"><strong>'+l.name+'</strong><div style="font-size:12px; color:#666">'+(l.native||'')+' • '+l.code+'</div></div>';
      it.addEventListener('click', ()=>{ localStorage.setItem('selectedLanguage', l.code); localStorage.setItem('selectedLanguageFlag', l.flag||'🏳️'); selectedFlagBtn.textContent = l.flag||'🏳️'; languageModal.style.display='none'; showToast('Lingua selezionata: '+l.name,1800); applyTranslations(); renderPrices(); });
      langListEl.appendChild(it);
    });
  }

  openLangBtn.addEventListener('click', ()=>{ renderLangList(''); languageModal.style.display='flex'; langSearch.value=''; langSearch.focus(); });
  closeLangModal.addEventListener('click', ()=> languageModal.style.display='none');
  langSearch.addEventListener('input', (e)=> renderLangList(e.target.value));
  // initialize selected flag from storage
  (function initSelectedLang(){ const s = localStorage.getItem('selectedLanguageFlag'); if (s) selectedFlagBtn.textContent = s; else { selectedFlagBtn.textContent = '🇮🇹'; localStorage.setItem('selectedLanguage','it'); localStorage.setItem('selectedLanguageFlag','🇮🇹'); } })();

  selectedFlagBtn.addEventListener('click', ()=>{ openLangBtn.click(); });

  // Intro overlay: show animation on page load (slides down from top then slides up)
  (function introOverlay(){
    try {
      const ov = document.createElement('div'); ov.id = 'introOverlay';
      ov.innerHTML = '<img src="https://scontent.fbri7-1.fna.fbcdn.net/v/t39.30808-6/299876829_584062196604180_7692658332015285145_n.jpg?_nc_cat=105&ccb=1-7&_nc_sid=6ee11a&_nc_ohc=C28QtqxSBQ0Q7kNvwHPVjsg&_nc_oc=AdlbogF4yalPoL9v93AffRPjVEMkgygRVTwZ2ZbuBrsEFZ8WAOCGo59Iw0p3A3luQFM&_nc_zt=23&_nc_ht=scontent.fbri7-1.fna&_nc_gid=BneWSvETip7O4-1tqn7hqw&oh=00_Afi50R0KveiNPFj090YvD6HcygOJRb8DG7a-RZdYtzKyzQ&oe=692A0AF9' + '" style="width:72px;height:72px;border-radius:8px;object-fit:cover;">' + '<div class="logo-large">Tendidea</div>';
      document.body.appendChild(ov);
      // slide down
      setTimeout(()=> ov.classList.add('show'), 80);
      // after 1.5s visible, slide up and remove
      setTimeout(()=>{ ov.classList.remove('show'); ov.classList.add('hidden'); setTimeout(()=>{ try{ ov.remove(); }catch(e){} }, 900); }, 1600);
    } catch(e){ console.warn('introOverlay failed', e); }
  })();

  // Defensive re-attachment of critical listeners (helps when earlier script sections fail)
  (function attachCriticalListeners(){
    // auth buttons
    addListener('loginBtn','click', ()=>{ const m = document.getElementById('loginModal'); if (m) m.style.display='flex'; });
    addListener('registerBtn','click', ()=>{ const m = document.getElementById('registerModal'); if (m) m.style.display='flex'; });

    // language
    addListener('openLangBtn','click', ()=>{ try{ renderLangList(''); languageModal.style.display='flex'; langSearch.value=''; langSearch.focus(); }catch(e){} });
    addListener('selectedFlagBtn','click', ()=>{ try{ openLangBtn && openLangBtn.click(); }catch(e){} });

    // ensure shipCountry reacts if present (in case populateCountrySelect wasn't called)
    addListener('shipCountry','change', (ev)=>{ try{ const sel = ev.target; const chosen = sel.options[sel.selectedIndex]; const cur = chosen && chosen.dataset && chosen.dataset.currency ? chosen.dataset.currency : (localStorage.getItem('selectedCurrency')||'EUR'); localStorage.setItem('selectedCountry', sel.value); localStorage.setItem('selectedCurrency', cur); const flag = chosen && chosen.dataset && chosen.dataset.flag ? chosen.dataset.flag : '🏳️'; const sfb = document.getElementById('selectedFlagBtn'); if (sfb) sfb.textContent = flag; applyTranslations(); renderPrices(); } catch(e){} });

    // card inputs (in case earlier binding failed)
    addListener('cardNumber','input', (e)=>{ try{ const v = e.target.value.replace(/\D/g, '').slice(0,19); const parts = []; for (let i=0;i<v.length;i+=4) parts.push(v.substr(i,4)); e.target.value = parts.join(' '); }catch(e){} });
    addListener('cardExp','input', (e)=>{ try{ const v = e.target.value.replace(/\D/g, '').slice(0,4); if (v.length >= 3) e.target.value = v.slice(0,2) + '/' + v.slice(2); else e.target.value = v; }catch(e){} });
    addListener('submitCard','click', (e)=>{ try{ e.preventDefault(); const name = document.getElementById('cardName')?.value.trim(); const number = (document.getElementById('cardNumber')?.value||'').replace(/\s/g,''); const exp = document.getElementById('cardExp')?.value.trim(); const cvc = document.getElementById('cardCvc')?.value.trim(); if (!name) { showToast('Inserisci nome titolare'); return; } if (!/^[0-9]{13,19}$/.test(number)) { showToast('Numero carta non valido'); return; } if (!/^(0[1-9]|1[0-2])\/[0-9]{2}$/.test(exp)) { showToast('Scadenza non valida (MM/AA)'); return; } if (!/^[0-9]{3,4}$/.test(cvc)) { showToast('CVC non valido'); return; } const cart = getCart(); const total = cart.reduce((s, it) => s + ((Number(it.price) || 0) * (Number(it.quantity) || 1)), 0); const btn = document.getElementById('submitCard'); if (btn){ btn.textContent = 'Elaborazione...'; btn.disabled = true; setTimeout(()=>{ btn.textContent = 'Paga'; btn.disabled = false; closeCheckout(); showToast(`Pagamento con carta eseguito: ${total.toFixed(2).replace('.', ',')} €`, 2800); saveCart([]); updateCartSummary(); document.getElementById('cardName').value=''; document.getElementById('cardNumber').value=''; document.getElementById('cardExp').value=''; document.getElementById('cardCvc').value=''; }, 1200); } }catch(e){} });

    // about/returns buttons
    addListener('aboutBtn','click', ()=>{ window.location.href = 'about.html'; });
    addListener('returnsRefundBtn','click', ()=>{ window.location.href = 'returns.html'; });

    // Mobile menu toggle and mobile-nav actions
    addListener('mobileMenuBtn','click', ()=>{ try{ const ov = document.getElementById('mobileNavOverlay'); if (ov) { ov.classList.add('open'); ov.setAttribute('aria-hidden','false'); } }catch(e){} });
    addListener('closeMobileNav','click', ()=>{ try{ const ov = document.getElementById('mobileNavOverlay'); if (ov) { ov.classList.remove('open'); ov.setAttribute('aria-hidden','true'); } }catch(e){} });
    // wire mobile nav buttons to same behaviors
    addListener('m_aboutBtn','click', ()=>{ try{ window.location.href = 'about.html'; }catch(e){} });
    addListener('m_returnsRefundBtn','click', ()=>{ try{ window.location.href = 'returns.html'; }catch(e){} });
    addListener('m_loginBtn','click', ()=>{ try{ const m = document.getElementById('loginModal'); const ov = document.getElementById('mobileNavOverlay'); if (ov) { ov.classList.remove('open'); ov.setAttribute('aria-hidden','true'); } if (m) m.style.display='flex'; }catch(e){} });
    addListener('m_registerBtn','click', ()=>{ try{ const m = document.getElementById('registerModal'); const ov = document.getElementById('mobileNavOverlay'); if (ov) { ov.classList.remove('open'); ov.setAttribute('aria-hidden','true'); } if (m) m.style.display='flex'; }catch(e){} });
  })();
</script>

  <!-- Footer aziendale -->
  <footer class="site-footer" aria-label="Informazioni aziendali">
    <div class="footer-inner">
      Via Dante 39 | 70016 | Noicattaro (BA) | C.F. PRTNGL73S16F923A | P. IVA 06776770726
    </div>
  </footer>

</body>
</html>
