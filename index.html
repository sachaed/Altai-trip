<!DOCTYPE html>

<html lang="fr">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Altaï — carnet de route · mai 2026</title>
<meta name="description" content="Road trip 8 jours dans les montagnes de l'Altaï, du 13 au 20 mai 2026." />

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,300;0,9..144,400;0,9..144,500;0,9..144,600;0,9..144,700;1,9..144,400&family=Inter:wght@300;400;500;600&family=JetBrains+Mono:wght@400;500&family=Vazirmatn:wght@300;400;500;600&display=swap" rel="stylesheet">

<!-- Leaflet for the map -->

<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"
      integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY="
      crossorigin=""/>
<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"
        integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo="
        crossorigin=""></script>

<style>
/* --------------------------------------------------------------
   Design tokens — travel-journal, warm paper, ink, a little worn
   -------------------------------------------------------------- */
:root {
  --paper: #f1e8d6;
  --paper-dark: #e4d7bc;
  --paper-shadow: #d9c7a5;
  --ink: #2a1f14;
  --ink-soft: #5a4632;
  --ink-faint: #8a7557;
  --accent: #b03a2e;       /* stamp red */
  --accent-2: #3f6b4f;     /* forest green */
  --accent-3: #1e4e6b;     /* cold river blue */
  --gold: #c08a3d;
  --rule: rgba(42,31,20,.18);
  --rule-strong: rgba(42,31,20,.45);
}

* { box-sizing: border-box; }
html, body { margin: 0; padding: 0; }
body {
  background: var(--paper);
  color: var(--ink);
  font-family: 'Fraunces', Georgia, serif;
  font-weight: 400;
  line-height: 1.6;
  font-size: 17px;
  -webkit-font-smoothing: antialiased;
  overflow-x: hidden;

  /* paper texture via layered gradients */
  background-image:
    radial-gradient(1200px 600px at 10% -10%, rgba(192,138,61,.12), transparent 60%),
    radial-gradient(900px 500px at 110% 20%, rgba(176,58,46,.08), transparent 60%),
    radial-gradient(800px 800px at 50% 110%, rgba(63,107,79,.08), transparent 60%);
}

/* Persian / Farsi styling */
html[lang="fa"] body { font-family: 'Vazirmatn', 'Fraunces', sans-serif; }
html[lang="fa"] .brand,
html[lang="fa"] .hero h1,
html[lang="fa"] .hero-sub,
html[lang="fa"] .section-title,
html[lang="fa"] .day-content h3,
html[lang="fa"] .day-subtitle,
html[lang="fa"] .footer-mark { font-family: 'Vazirmatn', sans-serif; }
html[lang="fa"] .hero h1 { font-weight: 400; line-height: 1.15; }
html[lang="fa"] .hero h1 .italic { font-style: normal; font-weight: 600; }
html[lang="fa"] .section-title .italic { font-style: normal; font-weight: 600; }
html[lang="fa"] .day-content h3 { font-weight: 500; }
html[lang="fa"] .day-subtitle { font-style: normal; }

/* Russian styling — Fraunces handles Cyrillic well */
html[lang="ru"] body { font-feature-settings: "ss01"; }

/* subtle paper grain overlay */
body::before {
  content: "";
  position: fixed; inset: 0;
  pointer-events: none;
  z-index: 1;
  background-image:
    repeating-linear-gradient(0deg, rgba(42,31,20,.015) 0 1px, transparent 1px 3px),
    repeating-linear-gradient(90deg, rgba(42,31,20,.015) 0 1px, transparent 1px 3px);
  mix-blend-mode: multiply;
  opacity: .6;
}

/* --------------------------------------------------------------
   Top bar
   -------------------------------------------------------------- */
.topbar {
  position: sticky; top: 0; z-index: 40;
  backdrop-filter: blur(8px);
  background: rgba(241, 232, 214, 0.82);
  border-bottom: 1px solid var(--rule);
  padding: 14px 28px;
  display: flex; align-items: center; justify-content: space-between;
  font-family: 'Inter', sans-serif;
  font-size: 13px;
  letter-spacing: .02em;
}
.brand {
  font-family: 'Fraunces', serif;
  font-weight: 600;
  font-style: italic;
  font-size: 18px;
  letter-spacing: -.01em;
}
.brand-dash { color: var(--accent); padding: 0 8px; }
.nav-links {
  display: flex; gap: 22px;
  list-style: none; padding: 0; margin: 0;
}
.nav-links a {
  color: var(--ink-soft); text-decoration: none;
  font-size: 13px;
  transition: color .2s;
  position: relative;
}
.nav-links a:hover { color: var(--accent); }
.nav-links a::after {
  content: ""; position: absolute; left: 0; bottom: -4px;
  width: 0; height: 1px; background: var(--accent);
  transition: width .25s;
}
.nav-links a:hover::after { width: 100%; }

/* Language toggle — dropdown style */
.lang-wrapper { position: relative; }
.lang-toggle {
  border: 1px solid var(--rule-strong);
  background: transparent;
  padding: 6px 14px;
  border-radius: 999px;
  cursor: pointer;
  font-family: 'Inter', sans-serif;
  font-size: 12px;
  color: var(--ink);
  letter-spacing: .12em;
  transition: all .2s;
  display: flex; align-items: center; gap: 6px;
}
.lang-toggle:hover { background: var(--ink); color: var(--paper); }
.lang-toggle .arrow { font-size: 9px; opacity: .6; }
.lang-menu {
  position: absolute;
  top: calc(100% + 6px);
  right: 0;
  background: var(--paper);
  border: 1px solid var(--rule-strong);
  border-radius: 8px;
  box-shadow: 0 12px 32px -8px rgba(42,31,20,.3);
  list-style: none;
  padding: 6px;
  margin: 0;
  min-width: 130px;
  display: none;
  z-index: 50;
}
.lang-menu.open { display: block; }
.lang-menu li button {
  width: 100%;
  text-align: left;
  background: transparent;
  border: none;
  padding: 8px 12px;
  border-radius: 4px;
  font-family: 'Inter', sans-serif;
  font-size: 13px;
  color: var(--ink-soft);
  cursor: pointer;
  display: flex; align-items: center; justify-content: space-between;
  gap: 10px;
  transition: background .15s;
}
.lang-menu li button:hover { background: rgba(42,31,20,.06); color: var(--ink); }
.lang-menu li button.active { background: rgba(176,58,46,.1); color: var(--accent); font-weight: 500; }
.lang-menu li button .code { font-family: 'JetBrains Mono', monospace; font-size: 11px; opacity: .5; letter-spacing: .1em; }

/* --------------------------------------------------------------
   Hero
   -------------------------------------------------------------- */
.hero {
  padding: 80px 28px 60px;
  max-width: 1100px;
  margin: 0 auto;
  position: relative;
  z-index: 2;
}
.hero-meta {
  font-family: 'Inter', sans-serif;
  font-size: 12px;
  text-transform: uppercase;
  letter-spacing: .28em;
  color: var(--ink-faint);
  margin-bottom: 24px;
  display: flex; align-items: center; gap: 14px;
}
.hero-meta::before, .hero-meta::after {
  content: ""; flex: 0 0 40px; height: 1px; background: var(--rule-strong);
}
html[lang="fa"] .hero-meta { text-transform: none; letter-spacing: .05em; font-size: 14px; }
html[lang="ru"] .hero-meta { letter-spacing: .18em; }

.hero h1 {
  font-family: 'Fraunces', serif;
  font-weight: 300;
  font-size: clamp(48px, 9vw, 120px);
  line-height: .95;
  letter-spacing: -.03em;
  margin: 0 0 24px;
}
.hero h1 .italic {
  font-style: italic;
  font-weight: 400;
  color: var(--accent);
}
.hero-sub {
  font-size: clamp(18px, 2vw, 22px);
  max-width: 620px;
  color: var(--ink-soft);
  line-height: 1.5;
  margin-bottom: 40px;
}
html[lang="fa"] .hero-sub { font-size: clamp(17px, 1.8vw, 20px); line-height: 1.7; }

.hero-stats {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 0;
  border-top: 1px solid var(--rule);
  border-bottom: 1px solid var(--rule);
  padding: 20px 0;
}
.hero-stats > div {
  border-right: 1px dashed var(--rule);
  padding: 0 20px;
}
.hero-stats > div:last-child { border-right: none; }
.hero-stats .label {
  font-family: 'Inter', sans-serif;
  font-size: 11px;
  text-transform: uppercase;
  letter-spacing: .18em;
  color: var(--ink-faint);
  margin-bottom: 6px;
}
html[lang="fa"] .hero-stats .label { font-family: 'Vazirmatn', sans-serif; text-transform: none; letter-spacing: 0; font-size: 13px; }
.hero-stats .value {
  font-family: 'Fraunces', serif;
  font-size: 28px;
  font-weight: 500;
  line-height: 1;
}
html[lang="fa"] .hero-stats .value { font-family: 'Vazirmatn', sans-serif; }
.hero-stats .value small { font-size: 14px; color: var(--ink-soft); font-weight: 400; margin-left: 4px; }

/* Decorative stamp */
.stamp {
  position: absolute;
  right: 40px;
  top: 90px;
  width: 150px; height: 150px;
  border: 2px solid var(--accent);
  border-radius: 50%;
  display: flex; align-items: center; justify-content: center;
  text-align: center;
  transform: rotate(-12deg);
  color: var(--accent);
  font-family: 'Fraunces', serif;
  font-style: italic;
  font-size: 13px;
  line-height: 1.3;
  opacity: .75;
  letter-spacing: .05em;
  padding: 12px;
}
.stamp::before {
  content: "";
  position: absolute; inset: 6px;
  border: 1px dashed var(--accent);
  border-radius: 50%;
}
.stamp strong {
  display: block;
  font-style: normal;
  font-weight: 700;
  font-size: 18px;
  letter-spacing: .1em;
  text-transform: uppercase;
  margin-bottom: 4px;
}

/* --------------------------------------------------------------
   Section headers
   -------------------------------------------------------------- */
section { position: relative; z-index: 2; }
.container { max-width: 1100px; margin: 0 auto; padding: 0 28px; }
.section-label {
  font-family: 'Inter', sans-serif;
  font-size: 11px;
  text-transform: uppercase;
  letter-spacing: .3em;
  color: var(--accent);
  margin-bottom: 14px;
  display: flex; align-items: center; gap: 12px;
}
.section-label::before {
  content: ""; width: 28px; height: 1px; background: var(--accent);
}
html[lang="fa"] .section-label { font-family: 'Vazirmatn', sans-serif; text-transform: none; letter-spacing: .05em; font-size: 13px; }
html[lang="ru"] .section-label { letter-spacing: .2em; }

.section-title {
  font-family: 'Fraunces', serif;
  font-weight: 400;
  font-size: clamp(36px, 5vw, 56px);
  line-height: 1.1;
  letter-spacing: -.02em;
  margin: 0 0 40px;
}
.section-title .italic { font-style: italic; color: var(--accent-3); }

/* --------------------------------------------------------------
   The journey — day cards
   -------------------------------------------------------------- */
.journey { padding: 80px 0 40px; }
.day {
  display: grid;
  grid-template-columns: 140px 1fr;
  gap: 40px;
  padding: 40px 0;
  border-top: 1px solid var(--rule);
  position: relative;
}
.day:last-child { border-bottom: 1px solid var(--rule); }

.day-index {
  font-family: 'Fraunces', serif;
  font-style: italic;
  color: var(--ink-faint);
}
.day-index .num {
  font-size: 72px;
  font-weight: 300;
  line-height: 1;
  display: block;
  color: var(--ink);
  font-style: normal;
  font-family: 'Fraunces', serif;
}
.day-index .date {
  font-family: 'Inter', sans-serif;
  font-size: 12px;
  letter-spacing: .1em;
  text-transform: uppercase;
  color: var(--ink-faint);
  margin-top: 6px;
  font-style: normal;
}

.day-content h3 {
  font-family: 'Fraunces', serif;
  font-weight: 500;
  font-size: 30px;
  margin: 0 0 6px;
  line-height: 1.15;
  letter-spacing: -.01em;
}
.day-subtitle {
  font-style: italic;
  color: var(--ink-soft);
  margin-bottom: 22px;
  font-size: 17px;
}
.day-image {
  width: 100%;
  aspect-ratio: 16/7;
  object-fit: cover;
  margin: 0 0 22px;
  border-radius: 2px;
  filter: sepia(.15) saturate(1.05);
  box-shadow:
    0 1px 0 var(--paper-shadow),
    0 20px 40px -20px rgba(42,31,20,.35);
}
.day-stops {
  list-style: none;
  padding: 0; margin: 0;
  display: grid;
  gap: 10px;
}
.day-stops li {
  display: grid;
  grid-template-columns: 80px 1fr;
  gap: 14px;
  padding: 10px 0;
  border-bottom: 1px dotted var(--rule);
  align-items: baseline;
}
.day-stops li:last-child { border-bottom: none; }
.stop-dist {
  font-family: 'JetBrains Mono', monospace;
  font-size: 12px;
  color: var(--accent);
  font-weight: 500;
  letter-spacing: .02em;
}
.stop-name {
  color: var(--ink);
}
.day-footer {
  margin-top: 20px;
  padding: 16px 20px;
  background: rgba(192, 138, 61, .08);
  border-left: 3px solid var(--gold);
  display: flex;
  flex-wrap: wrap;
  gap: 18px;
  font-size: 14px;
  font-family: 'Inter', sans-serif;
  color: var(--ink-soft);
}
html[lang="fa"] .day-footer { font-family: 'Vazirmatn', sans-serif; font-size: 14px; }
.day-footer span strong {
  color: var(--ink);
  font-weight: 500;
}
.day-footer .payment-paid { color: var(--accent-2); font-weight: 500; }
.day-footer .payment-unpaid { color: var(--accent); font-weight: 500; }

/* RTL adjustments for Persian */
html[dir="rtl"] .day { grid-template-columns: 1fr 140px; }
html[dir="rtl"] .day-index { text-align: left; }
html[dir="rtl"] .day-stops li { grid-template-columns: 1fr 80px; }
html[dir="rtl"] .stop-dist { text-align: left; }
html[dir="rtl"] .day-footer { border-left: none; border-right: 3px solid var(--gold); }
html[dir="rtl"] .section-label::before { display: none; }
html[dir="rtl"] .section-label::after { content: ""; width: 28px; height: 1px; background: var(--accent); }
html[dir="rtl"] .stamp { right: auto; left: 40px; transform: rotate(12deg); }
html[dir="rtl"] .nav-links a::after { left: auto; right: 0; }
html[dir="rtl"] .lang-menu { right: auto; left: 0; }
html[dir="rtl"] .budget-card::before { right: -1px; }
html[dir="rtl"] .hero-stats .value small { margin-left: 0; margin-right: 4px; }
html[dir="rtl"] .budget-amount .currency { margin-left: 0; margin-right: 4px; }

/* --------------------------------------------------------------
   Map section
   -------------------------------------------------------------- */
.map-section { padding: 80px 0; }
#map {
  height: 520px;
  width: 100%;
  border: 1px solid var(--rule-strong);
  box-shadow: 0 30px 60px -30px rgba(42,31,20,.4);
  filter: sepia(.12) saturate(.85);
}
.map-legend {
  margin-top: 16px;
  font-family: 'Inter', sans-serif;
  font-size: 12px;
  color: var(--ink-faint);
  font-style: italic;
  text-align: center;
}
html[lang="fa"] .map-legend { font-family: 'Vazirmatn', sans-serif; font-style: normal; }

/* --------------------------------------------------------------
   Budget
   -------------------------------------------------------------- */
.budget-section { padding: 80px 0; background: rgba(42,31,20,.03); }
.budget-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 24px;
  margin-bottom: 30px;
}
.budget-card {
  padding: 28px 24px;
  background: var(--paper);
  border: 1px solid var(--rule);
  position: relative;
}
.budget-card::before {
  content: "";
  position: absolute;
  top: -1px; left: -1px; right: -1px;
  height: 3px;
  background: var(--accent);
}
.budget-card:nth-child(2)::before { background: var(--accent-2); }
.budget-card:nth-child(3)::before { background: var(--accent-3); }
.budget-card:nth-child(4)::before { background: var(--gold); }

.budget-label {
  font-family: 'Inter', sans-serif;
  font-size: 11px;
  text-transform: uppercase;
  letter-spacing: .2em;
  color: var(--ink-faint);
  margin-bottom: 10px;
}
html[lang="fa"] .budget-label { font-family: 'Vazirmatn', sans-serif; text-transform: none; letter-spacing: 0; font-size: 13px; }
.budget-amount {
  font-family: 'Fraunces', serif;
  font-size: 36px;
  font-weight: 500;
  line-height: 1;
  letter-spacing: -.02em;
}
.budget-amount .currency {
  font-size: 20px;
  font-weight: 400;
  color: var(--ink-soft);
  margin-left: 4px;
}
.budget-total {
  padding: 28px;
  background: var(--ink);
  color: var(--paper);
  display: flex; align-items: baseline; justify-content: space-between;
}
.budget-total .label {
  font-family: 'Inter', sans-serif;
  font-size: 13px;
  text-transform: uppercase;
  letter-spacing: .22em;
}
html[lang="fa"] .budget-total .label { font-family: 'Vazirmatn', sans-serif; text-transform: none; letter-spacing: 0; font-size: 15px; }
.budget-total .amount {
  font-family: 'Fraunces', serif;
  font-weight: 400;
  font-size: 46px;
  letter-spacing: -.02em;
}
.budget-total .amount .currency { font-size: 24px; opacity: .7; margin-left: 6px; }

/* --------------------------------------------------------------
   Summary table
   -------------------------------------------------------------- */
.recap-section { padding: 80px 0; }
.recap-wrapper {
  border: 1px solid var(--rule-strong);
  overflow-x: auto;
}
table.recap {
  width: 100%;
  border-collapse: collapse;
  font-family: 'Inter', sans-serif;
  font-size: 14px;
  background: var(--paper);
}
html[lang="fa"] table.recap { font-family: 'Vazirmatn', sans-serif; }
table.recap th {
  text-align: left;
  padding: 16px 18px;
  font-weight: 500;
  font-size: 11px;
  text-transform: uppercase;
  letter-spacing: .2em;
  color: var(--ink-faint);
  border-bottom: 1px solid var(--rule-strong);
  background: rgba(42,31,20,.04);
  white-space: nowrap;
}
html[dir="rtl"] table.recap th { text-align: right; }
html[lang="fa"] table.recap th { text-transform: none; letter-spacing: 0; font-size: 13px; }
table.recap td {
  padding: 14px 18px;
  border-bottom: 1px solid var(--rule);
  vertical-align: top;
}
table.recap tr:last-child td { border-bottom: none; }
table.recap tr.total-row td {
  font-weight: 600;
  background: rgba(42,31,20,.06);
  border-top: 2px solid var(--ink);
  font-family: 'Fraunces', serif;
  font-size: 16px;
  font-style: italic;
}
html[lang="fa"] table.recap tr.total-row td { font-family: 'Vazirmatn', sans-serif; font-style: normal; font-weight: 600; }
table.recap td.day-num {
  font-family: 'Fraunces', serif;
  font-style: italic;
  color: var(--accent);
  font-weight: 500;
  font-size: 18px;
}
table.recap td.km-num {
  font-family: 'JetBrains Mono', monospace;
  font-weight: 500;
}

/* --------------------------------------------------------------
   Footer
   -------------------------------------------------------------- */
footer {
  padding: 60px 28px 40px;
  text-align: center;
  font-family: 'Inter', sans-serif;
  color: var(--ink-faint);
  font-size: 12px;
  letter-spacing: .05em;
  position: relative; z-index: 2;
}
html[lang="fa"] footer { font-family: 'Vazirmatn', sans-serif; }
footer .heart { color: var(--accent); }
footer .footer-mark {
  font-family: 'Fraunces', serif;
  font-style: italic;
  font-size: 16px;
  color: var(--ink-soft);
  margin-bottom: 8px;
}

/* --------------------------------------------------------------
   Responsive
   -------------------------------------------------------------- */
@media (max-width: 820px) {
  .stamp { display: none; }
  .hero { padding: 50px 22px 40px; }
  .hero-stats { grid-template-columns: repeat(2, 1fr); }
  .hero-stats > div:nth-child(2) { border-right: none; }
  .hero-stats > div:nth-child(1), .hero-stats > div:nth-child(2) {
    border-bottom: 1px dashed var(--rule);
    padding-bottom: 16px; margin-bottom: 16px;
  }
  .day { grid-template-columns: 1fr; gap: 16px; padding: 30px 0; }
  html[dir="rtl"] .day { grid-template-columns: 1fr; }
  .day-index .num { font-size: 52px; }
  .day-content h3 { font-size: 24px; }
  .budget-grid { grid-template-columns: 1fr 1fr; }
  .container { padding: 0 22px; }
  .nav-links { display: none; }
  .topbar { padding: 12px 18px; }
}
@media (max-width: 480px) {
  .budget-grid { grid-template-columns: 1fr; }
  .day-stops li { grid-template-columns: 70px 1fr; gap: 10px; }
  html[dir="rtl"] .day-stops li { grid-template-columns: 1fr 70px; }
}

/* --------------------------------------------------------------
   Entrance animation
   -------------------------------------------------------------- */
@keyframes fadeRise {
  from { opacity: 0; transform: translateY(16px); }
  to { opacity: 1; transform: none; }
}
.hero h1, .hero-sub, .hero-meta, .hero-stats, .stamp {
  animation: fadeRise .9s ease both;
}
.hero-meta { animation-delay: .05s; }
.hero h1 { animation-delay: .15s; }
.hero-sub { animation-delay: .3s; }
.hero-stats { animation-delay: .45s; }
.stamp { animation-delay: .8s; }

/* Hidden i18n variants */
[data-lang]:not(.active) { display: none; }
</style>

</head>
<body>

<!-- ============================================================
     TOP BAR
     ============================================================ -->

<header class="topbar">
  <div class="brand">
    <span data-lang="fr" class="active">Altaï<span class="brand-dash">·</span>carnet de route</span>
    <span data-lang="en">Altai<span class="brand-dash">·</span>road journal</span>
    <span data-lang="ru">Алтай<span class="brand-dash">·</span>путевой дневник</span>
    <span data-lang="fa">آلتای<span class="brand-dash">·</span>دفترچه سفر</span>
  </div>
  <nav>
    <ul class="nav-links">
      <li><a href="#journey">
        <span data-lang="fr" class="active">Le voyage</span>
        <span data-lang="en">The journey</span>
        <span data-lang="ru">Путешествие</span>
        <span data-lang="fa">سفر</span>
      </a></li>
      <li><a href="#map-section">
        <span data-lang="fr" class="active">Carte</span>
        <span data-lang="en">Map</span>
        <span data-lang="ru">Карта</span>
        <span data-lang="fa">نقشه</span>
      </a></li>
      <li><a href="#budget">
        <span data-lang="fr" class="active">Budget</span>
        <span data-lang="en">Budget</span>
        <span data-lang="ru">Бюджет</span>
        <span data-lang="fa">بودجه</span>
      </a></li>
      <li><a href="#recap">
        <span data-lang="fr" class="active">Récap</span>
        <span data-lang="en">Summary</span>
        <span data-lang="ru">Сводка</span>
        <span data-lang="fa">خلاصه</span>
      </a></li>
    </ul>
  </nav>
  <div class="lang-wrapper">
    <button class="lang-toggle" id="langToggle" aria-label="Change language">
      <span id="lang-current">FR</span>
      <span class="arrow">▼</span>
    </button>
    <ul class="lang-menu" id="langMenu">
      <li><button data-set-lang="fr" class="active">Français <span class="code">FR</span></button></li>
      <li><button data-set-lang="en">English <span class="code">EN</span></button></li>
      <li><button data-set-lang="ru">Русский <span class="code">RU</span></button></li>
      <li><button data-set-lang="fa">فارسی <span class="code">FA</span></button></li>
    </ul>
  </div>
</header>

<!-- ============================================================
     HERO
     ============================================================ -->

<section class="hero">
  <div class="stamp">
    <div>
      <strong>Altaï</strong>
      <span data-lang="fr" class="active">Mai 2026 · 8 jours</span>
      <span data-lang="en">May 2026 · 8 days</span>
      <span data-lang="ru">Май 2026 · 8 дней</span>
      <span data-lang="fa">می ۲۰۲۶ · ۸ روز</span>
    </div>
  </div>
  <div class="hero-meta">
    <span data-lang="fr" class="active">Carnet de voyage · Sibérie · Mai 2026</span>
    <span data-lang="en">Travel journal · Siberia · May 2026</span>
    <span data-lang="ru">Путевой дневник · Сибирь · Май 2026</span>
    <span data-lang="fa">دفترچه سفر · سیبری · می ۲۰۲۶</span>
  </div>
  <h1>
    <span data-lang="fr" class="active">Altaï,<br><span class="italic">huit jours</span> de route</span>
    <span data-lang="en">Altai,<br><span class="italic">eight days</span> on the road</span>
    <span data-lang="ru">Алтай,<br><span class="italic">восемь дней</span> в пути</span>
    <span data-lang="fa">آلتای،<br><span class="italic">هشت روز</span> در جاده</span>
  </h1>
  <p class="hero-sub">
    <span data-lang="fr" class="active">Un road trip entre cols, cascades et confluences turquoise — de Gorno-Altaïsk aux montagnes de la Chuya, du 13 au 20 mai.</span>
    <span data-lang="en">A road trip through passes, waterfalls and turquoise confluences — from Gorno-Altaysk to the Chuya mountains, May 13–20.</span>
    <span data-lang="ru">Путешествие через перевалы, водопады и бирюзовые слияния рек — от Горно-Алтайска до гор Чуи, с 13 по 20 мая.</span>
    <span data-lang="fa">یک سفر جاده‌ای میان گردنه‌ها، آبشارها و تلاقی‌های فیروزه‌ای — از گورنو-آلتایسک تا کوه‌های چویا، از ۱۳ تا ۲۰ می.</span>
  </p>
  <div class="hero-stats">
    <div>
      <div class="label">
        <span data-lang="fr" class="active">Kilomètres</span>
        <span data-lang="en">Kilometres</span>
        <span data-lang="ru">Километры</span>
        <span data-lang="fa">کیلومتر</span>
      </div>
      <div class="value">1 150<small>km</small></div>
    </div>
    <div>
      <div class="label">
        <span data-lang="fr" class="active">Jours</span>
        <span data-lang="en">Days</span>
        <span data-lang="ru">Дни</span>
        <span data-lang="fa">روزها</span>
      </div>
      <div class="value">8</div>
    </div>
    <div>
      <div class="label">
        <span data-lang="fr" class="active">Étapes</span>
        <span data-lang="en">Stops</span>
        <span data-lang="ru">Остановки</span>
        <span data-lang="fa">توقف‌ها</span>
      </div>
      <div class="value">20+</div>
    </div>
    <div>
      <div class="label">
        <span data-lang="fr" class="active">Budget</span>
        <span data-lang="en">Budget</span>
        <span data-lang="ru">Бюджет</span>
        <span data-lang="fa">بودجه</span>
      </div>
      <div class="value">128 800<small>₽</small></div>
    </div>
  </div>
</section>

<!-- ============================================================
     JOURNEY
     ============================================================ -->

<section class="journey" id="journey">
  <div class="container">
    <div class="section-label">
      <span data-lang="fr" class="active">I · Le voyage</span>
      <span data-lang="en">I · The journey</span>
      <span data-lang="ru">I · Путешествие</span>
      <span data-lang="fa">۱ · سفر</span>
    </div>
    <h2 class="section-title">
      <span data-lang="fr" class="active">Jour après jour, <span class="italic">étape par étape</span></span>
      <span data-lang="en">Day by day, <span class="italic">stop by stop</span></span>
      <span data-lang="ru">День за днём, <span class="italic">остановка за остановкой</span></span>
      <span data-lang="fa">روز به روز، <span class="italic">توقف به توقف</span></span>
    </h2>

```
<!-- DAY 1 -->
<article class="day">
  <div class="day-index">
    <span class="num">01</span>
    <span class="date">13 · 05 · 2026</span>
  </div>
  <div class="day-content">
    <h3>
      <span data-lang="fr" class="active">Arrivée &amp; premiers pas dans l'Altaï</span>
      <span data-lang="en">Arrival &amp; first steps in Altai</span>
      <span data-lang="ru">Прибытие и первые шаги по Алтаю</span>
      <span data-lang="fa">ورود و نخستین گام‌ها در آلتای</span>
    </h3>
    <div class="day-subtitle">
      <span data-lang="fr" class="active">Récupération de la voiture à l'aéroport — puis cap sur les premières curiosités.</span>
      <span data-lang="en">Pick up the car at the airport — then aim for the first wonders.</span>
      <span data-lang="ru">Получаем машину в аэропорту — и едем к первым достопримечательностям.</span>
      <span data-lang="fa">تحویل خودرو در فرودگاه — و سپس به سوی نخستین جاذبه‌ها.</span>
    </div>
    <ul class="day-stops">
      <li><span class="stop-dist">— km</span><span class="stop-name">
        <span data-lang="fr" class="active">Récupération de la voiture à l'aéroport</span>
        <span data-lang="en">Pick up the car at the airport</span>
        <span data-lang="ru">Получение автомобиля в аэропорту</span>
        <span data-lang="fa">تحویل خودرو در فرودگاه</span>
      </span></li>
      <li><span class="stop-dist">Chertov</span><span class="stop-name">
        <span data-lang="fr" class="active">« Doigt du Diable » (Chertov Palets)</span>
        <span data-lang="en">"Devil's Finger" (Chertov Palets)</span>
        <span data-lang="ru">Чёртов палец</span>
        <span data-lang="fa">«انگشت شیطان» (چرتوف پالتس)</span>
      </span></li>
      <li><span class="stop-dist">Porogi</span><span class="stop-name">
        <span data-lang="fr" class="active">Rapides de Manzherok</span>
        <span data-lang="en">Manzherok rapids</span>
        <span data-lang="ru">Манжерокские пороги</span>
        <span data-lang="fa">تندآب‌های مانژروک</span>
      </span></li>
      <li><span class="stop-dist">1h walk</span><span class="stop-name">
        <span data-lang="fr" class="active">Cascade de Kamishlinsky</span>
        <span data-lang="en">Kamishlinsky waterfall</span>
        <span data-lang="ru">Камышлинский водопад</span>
        <span data-lang="fa">آبشار کامیشلینسکی</span>
      </span></li>
    </ul>
    <div class="day-footer">
      <span>🛏 <strong>Loft 12</strong></span>
      <span>6 880 ₽ · 
        <span data-lang="fr" class="active">petit-déj inclus</span>
        <span data-lang="en">breakfast included</span>
        <span data-lang="ru">завтрак включён</span>
        <span data-lang="fa">صبحانه شامل</span>
      </span>
      <span class="payment-paid">✓ 
        <span data-lang="fr" class="active">Payé</span>
        <span data-lang="en">Paid</span>
        <span data-lang="ru">Оплачено</span>
        <span data-lang="fa">پرداخت شده</span>
      </span>
      <span>🚗 60 km</span>
    </div>
  </div>
</article>

<!-- DAY 2 -->
<article class="day">
  <div class="day-index">
    <span class="num">02</span>
    <span class="date">14 · 05 · 2026</span>
  </div>
  <div class="day-content">
    <h3>
      <span data-lang="fr" class="active">Col de Seminsky &amp; cascade</span>
      <span data-lang="en">Seminsky pass &amp; waterfall</span>
      <span data-lang="ru">Семинский перевал и водопад</span>
      <span data-lang="fa">گردنه سمینسکی و آبشار</span>
    </h3>
    <div class="day-subtitle">
      <span data-lang="fr" class="active">Grande journée de route — on monte en altitude et on trouve Arbat pour la nuit.</span>
      <span data-lang="en">A long road day — climbing into the highlands, Arbat for the night.</span>
      <span data-lang="ru">Долгий день в дороге — поднимаемся в горы, ночуем в Арбате.</span>
      <span data-lang="fa">روزی طولانی در جاده — به ارتفاعات می‌رویم، شب را در آرباط می‌گذرانیم.</span>
    </div>
    <ul class="day-stops">
      <li><span class="stop-dist">87 km</span><span class="stop-name">
        <span data-lang="fr" class="active">Col de Seminsky (Seminsky Pereval)</span>
        <span data-lang="en">Seminsky Pass</span>
        <span data-lang="ru">Семинский перевал</span>
        <span data-lang="fa">گردنه سمینسکی</span>
      </span></li>
      <li><span class="stop-dist">90 km</span><span class="stop-name">
        <span data-lang="fr" class="active">Cascade &amp; pristan</span>
        <span data-lang="en">Waterfall &amp; pristan</span>
        <span data-lang="ru">Водопад и пристань</span>
        <span data-lang="fa">آبشار و اسکله</span>
      </span></li>
      <li><span class="stop-dist">24 km</span><span class="stop-name">
        <span data-lang="fr" class="active">Hôtel Arbat (maison n°7)</span>
        <span data-lang="en">Arbat hotel (house #7)</span>
        <span data-lang="ru">Отель Арбат (дом №7)</span>
        <span data-lang="fa">هتل آرباط (خانه شماره ۷)</span>
      </span></li>
    </ul>
    <div class="day-footer">
      <span>🛏 <strong>Arbat · 
        <span data-lang="fr" class="active">maison 7</span>
        <span data-lang="en">house 7</span>
        <span data-lang="ru">дом 7</span>
        <span data-lang="fa">خانه ۷</span>
      </strong></span>
      <span>6 500 ₽</span>
      <span class="payment-unpaid">⚠ 
        <span data-lang="fr" class="active">À payer — en espèces</span>
        <span data-lang="en">Unpaid — bring cash</span>
        <span data-lang="ru">Не оплачено — наличными</span>
        <span data-lang="fa">پرداخت نشده — نقدی همراه ببرید</span>
      </span>
      <span>🚗 200 km</span>
    </div>
  </div>
</article>

<!-- DAY 3 -->
<article class="day">
  <div class="day-index">
    <span class="num">03</span>
    <span class="date">15 · 05 · 2026</span>
  </div>
  <div class="day-content">
    <h3>
      <span data-lang="fr" class="active">La confluence turquoise</span>
      <span data-lang="en">The turquoise confluence</span>
      <span data-lang="ru">Бирюзовое слияние рек</span>
      <span data-lang="fa">تلاقی فیروزه‌ای</span>
    </h3>
    <div class="day-subtitle">
      <span data-lang="fr" class="active">Le clou du voyage : Chuya + Katun, là où les deux rivières se rencontrent sans se mélanger.</span>
      <span data-lang="en">The highlight: Chuya + Katun, where two rivers meet without mixing.</span>
      <span data-lang="ru">Гвоздь поездки: Чуя и Катунь — место, где две реки встречаются, не смешиваясь.</span>
      <span data-lang="fa">نقطه اوج سفر: چویا + کاتون، جایی که دو رودخانه به هم می‌رسند بی‌آنکه درآمیزند.</span>
    </div>
    <ul class="day-stops">
      <li><span class="stop-dist">10 km</span><span class="stop-name">
        <span data-lang="fr" class="active">Col de Chike-Taman</span>
        <span data-lang="en">Chike-Taman Pass</span>
        <span data-lang="ru">Перевал Чике-Таман</span>
        <span data-lang="fa">گردنه چیکه-تامان</span>
      </span></li>
      <li><span class="stop-dist">20 km</span><span class="stop-name">
        <span data-lang="fr" class="active">Rapides d'Ilgumensky</span>
        <span data-lang="en">Ilgumensky rapids</span>
        <span data-lang="ru">Ильгуменский порог</span>
        <span data-lang="fa">تندآب ایلگومنسکی</span>
      </span></li>
      <li><span class="stop-dist">35 km</span><span class="stop-name">
        <span data-lang="fr" class="active">Confluence Chuya + Katun</span>
        <span data-lang="en">Chuya + Katun confluence</span>
        <span data-lang="ru">Слияние Чуи и Катуни</span>
        <span data-lang="fa">تلاقی چویا و کاتون</span>
      </span></li>
      <li><span class="stop-dist">50 km</span><span class="stop-name">
        <span data-lang="fr" class="active">Cascade de Shirlak &amp; rapides de Begemot</span>
        <span data-lang="en">Shirlak waterfall &amp; Begemot rapids</span>
        <span data-lang="ru">Водопад Ширлак и порог Бегемот</span>
        <span data-lang="fa">آبشار شیرلاک و تندآب بگموت</span>
      </span></li>
      <li><span class="stop-dist">30 km</span><span class="stop-name">
        <span data-lang="fr" class="active">Green Kolobok</span>
        <span data-lang="en">Green Kolobok</span>
        <span data-lang="ru">Зелёный Колобок</span>
        <span data-lang="fa">گرین کولوبوک</span>
      </span></li>
    </ul>
    <div class="day-footer">
      <span>🛏 <strong>Green Kolobok</strong></span>
      <span>5 900 ₽ / 
        <span data-lang="fr" class="active">nuit · total 2 nuits : 11 800 ₽</span>
        <span data-lang="en">night · total 2 nights: 11 800 ₽</span>
        <span data-lang="ru">ночь · всего за 2 ночи: 11 800 ₽</span>
        <span data-lang="fa">شب · مجموع ۲ شب: ۱۱٬۸۰۰ ₽</span>
      </span>
      <span class="payment-paid">✓ 
        <span data-lang="fr" class="active">1 000 ₽ d'acompte versé</span>
        <span data-lang="en">1 000 ₽ deposit paid</span>
        <span data-lang="ru">Внесён задаток 1 000 ₽</span>
        <span data-lang="fa">۱٬۰۰۰ ₽ بیعانه پرداخت شده</span>
      </span>
      <span>🚗 150 km</span>
    </div>
  </div>
</article>

<!-- DAY 4 -->
<article class="day">
  <div class="day-index">
    <span class="num">04</span>
    <span class="date">16 · 05 · 2026</span>
  </div>
  <div class="day-content">
    <h3>
      <span data-lang="fr" class="active">Trek &amp; lac Geyser</span>
      <span data-lang="en">Trek &amp; Geyser lake</span>
      <span data-lang="ru">Поход и Гейзеровое озеро</span>
      <span data-lang="fa">پیاده‌روی و دریاچه گیزر</span>
    </h3>
    <div class="day-subtitle">
      <span data-lang="fr" class="active">Journée rando — et en chemin, on s'arrête au mystérieux lac Geyser aux cercles bleus.</span>
      <span data-lang="en">Hiking day — on the way back, a stop at the mysterious blue-circle Geyser Lake.</span>
      <span data-lang="ru">День похода — на обратном пути остановка у загадочного Гейзерового озера с синими кругами.</span>
      <span data-lang="fa">روز کوهنوردی — در راه بازگشت، توقفی در دریاچه مرموز گیزر با دایره‌های آبی.</span>
    </div>
    <ul class="day-stops">
      <li><span class="stop-dist">70 km</span><span class="stop-name">
        <span data-lang="fr" class="active">Rando en montagne</span>
        <span data-lang="en">Mountain trek</span>
        <span data-lang="ru">Горный поход</span>
        <span data-lang="fa">کوهنوردی</span>
      </span></li>
      <li><span class="stop-dist">—</span><span class="stop-name">
        <span data-lang="fr" class="active">Lac Geyser (arrêt au retour)</span>
        <span data-lang="en">Geyser Lake (stop on the way back)</span>
        <span data-lang="ru">Гейзеровое озеро (остановка на обратном пути)</span>
        <span data-lang="fa">دریاچه گیزر (توقف در راه بازگشت)</span>
      </span></li>
    </ul>
    <div class="day-footer">
      <span>🛏 <strong>Green Kolobok</strong> (
        <span data-lang="fr" class="active">2e nuit</span>
        <span data-lang="en">2nd night</span>
        <span data-lang="ru">2-я ночь</span>
        <span data-lang="fa">شب دوم</span>
      )</span>
      <span class="payment-paid">✓ 
        <span data-lang="fr" class="active">incluse dans les 11 800 ₽</span>
        <span data-lang="en">included in 11 800 ₽</span>
        <span data-lang="ru">входит в 11 800 ₽</span>
        <span data-lang="fa">در ۱۱٬۸۰۰ ₽ گنجانده شده</span>
      </span>
      <span>🚗 150 km</span>
    </div>
  </div>
</article>

<!-- DAY 5 -->
<article class="day">
  <div class="day-index">
    <span class="num">05</span>
    <span class="date">17 · 05 · 2026</span>
  </div>
  <div class="day-content">
    <h3>
      <span data-lang="fr" class="active">Grand retour plein nord</span>
      <span data-lang="en">The long road back, north</span>
      <span data-lang="ru">Долгое возвращение на север</span>
      <span data-lang="fa">بازگشت طولانی به سمت شمال</span>
    </h3>
    <div class="day-subtitle">
      <span data-lang="fr" class="active">300 km d'une traite pour retrouver Loft 12 — la route la plus longue du voyage.</span>
      <span data-lang="en">300 km in one go back to Loft 12 — the longest drive of the trip.</span>
      <span data-lang="ru">300 км за один раз обратно в Loft 12 — самый длинный отрезок поездки.</span>
      <span data-lang="fa">۳۰۰ کیلومتر یک‌سره تا لافت ۱۲ — طولانی‌ترین مسیر سفر.</span>
    </div>
    <ul class="day-stops">
      <li><span class="stop-dist">300 km</span><span class="stop-name">
        <span data-lang="fr" class="active">Green Kolobok → Loft 12</span>
        <span data-lang="en">Green Kolobok → Loft 12</span>
        <span data-lang="ru">Зелёный Колобок → Loft 12</span>
        <span data-lang="fa">گرین کولوبوک ← لافت ۱۲</span>
      </span></li>
    </ul>
    <div class="day-footer">
      <span>🛏 <strong>Loft 12</strong></span>
      <span>6 880 ₽ · 
        <span data-lang="fr" class="active">petit-déj inclus</span>
        <span data-lang="en">breakfast included</span>
        <span data-lang="ru">завтрак включён</span>
        <span data-lang="fa">صبحانه شامل</span>
      </span>
      <span class="payment-paid">✓ 
        <span data-lang="fr" class="active">Payé</span>
        <span data-lang="en">Paid</span>
        <span data-lang="ru">Оплачено</span>
        <span data-lang="fa">پرداخت شده</span>
      </span>
      <span>🚗 300 km</span>
    </div>
  </div>
</article>

<!-- DAY 6 -->
<article class="day">
  <div class="day-index">
    <span class="num">06</span>
    <span class="date">18 · 05 · 2026</span>
  </div>
  <div class="day-content">
    <h3>
      <span data-lang="fr" class="active">Île de Patmos &amp; gorge Che-Chkysh</span>
      <span data-lang="en">Patmos Island &amp; Che-Chkysh gorge</span>
      <span data-lang="ru">Остров Патмос и ущелье Че-Чкыш</span>
      <span data-lang="fa">جزیره پاتموس و دره چه-چکیش</span>
    </h3>
    <div class="day-subtitle">
      <span data-lang="fr" class="active">Rochers du Dragon, petite île-monastère suspendue, cascades — une journée en cartes postales.</span>
      <span data-lang="en">Dragon rocks, a tiny suspended monastery-island, waterfalls — a postcard day.</span>
      <span data-lang="ru">Скалы Дракона, маленький подвесной остров-монастырь, водопады — день как открытка.</span>
      <span data-lang="fa">صخره‌های اژدها، جزیره-صومعه‌ی کوچک معلق، آبشارها — روزی چون کارت‌پستال.</span>
    </div>
    <ul class="day-stops">
      <li><span class="stop-dist">30 km</span><span class="stop-name">
        <span data-lang="fr" class="active">Rochers du Dragon</span>
        <span data-lang="en">Dragon Rocks</span>
        <span data-lang="ru">Скалы Дракона</span>
        <span data-lang="fa">صخره‌های اژدها</span>
      </span></li>
      <li><span class="stop-dist">10 km</span><span class="stop-name">
        <span data-lang="fr" class="active">Île de Patmos + points de vue</span>
        <span data-lang="en">Patmos Island + viewpoints</span>
        <span data-lang="ru">Остров Патмос и смотровые площадки</span>
        <span data-lang="fa">جزیره پاتموس + نقاط دید</span>
      </span></li>
      <li><span class="stop-dist">15 km</span><span class="stop-name">
        <span data-lang="fr" class="active">Cascade Che-Chkysh</span>
        <span data-lang="en">Che-Chkysh waterfall</span>
        <span data-lang="ru">Водопад Че-Чкыш</span>
        <span data-lang="fa">آبشار چه-چکیش</span>
      </span></li>
      <li><span class="stop-dist">80 km</span><span class="stop-name">Manzherok</span></li>
    </ul>
    <div class="day-footer">
      <span>🛏 <strong>
        <span data-lang="fr" class="active">Hôtel Geometrika</span>
        <span data-lang="en">Geometrika Hotel</span>
        <span data-lang="ru">Отель Геометрика</span>
        <span data-lang="fa">هتل گئومتریکا</span>
      </strong></span>
      <span>15 200 ₽</span>
      <span class="payment-paid">✓ 
        <span data-lang="fr" class="active">Payé</span>
        <span data-lang="en">Paid</span>
        <span data-lang="ru">Оплачено</span>
        <span data-lang="fa">پرداخت شده</span>
      </span>
      <span>🚗 135 km</span>
    </div>
  </div>
</article>

<!-- DAY 7 -->
<article class="day">
  <div class="day-index">
    <span class="num">07</span>
    <span class="date">19 · 05 · 2026</span>
  </div>
  <div class="day-content">
    <h3>
      <span data-lang="fr" class="active">Dernière balade &amp; retour vers l'aéroport</span>
      <span data-lang="en">Last walk &amp; back to the airport</span>
      <span data-lang="ru">Последняя прогулка и возвращение в аэропорт</span>
      <span data-lang="fa">آخرین قدم‌زدن و بازگشت به فرودگاه</span>
    </h3>
    <div class="day-subtitle">
      <span data-lang="fr" class="active">Promenade à Manzherok, petit détour lavage auto, et nuit tout près du terminal.</span>
      <span data-lang="en">A walk in Manzherok, a car wash detour, and a night right next to the terminal.</span>
      <span data-lang="ru">Прогулка в Манжероке, заезд на мойку и ночёвка рядом с терминалом.</span>
      <span data-lang="fa">قدم‌زنی در مانژروک، توقفی در کارواش و شبی نزدیک ترمینال.</span>
    </div>
    <ul class="day-stops">
      <li><span class="stop-dist">—</span><span class="stop-name">
        <span data-lang="fr" class="active">Promenade à Manzherok</span>
        <span data-lang="en">Walk in Manzherok</span>
        <span data-lang="ru">Прогулка в Манжероке</span>
        <span data-lang="fa">قدم‌زنی در مانژروک</span>
      </span></li>
      <li><span class="stop-dist">30 km</span><span class="stop-name">
        <span data-lang="fr" class="active">Route vers Gorno-Altaïsk</span>
        <span data-lang="en">Road to Gorno-Altaysk</span>
        <span data-lang="ru">Дорога в Горно-Алтайск</span>
        <span data-lang="fa">جاده به سوی گورنو-آلتایسک</span>
      </span></li>
      <li><span class="stop-dist">—</span><span class="stop-name">
        <span data-lang="fr" class="active">Lavage de la voiture</span>
        <span data-lang="en">Wash the car</span>
        <span data-lang="ru">Мойка машины</span>
        <span data-lang="fa">شستن خودرو</span>
      </span></li>
    </ul>
    <div class="day-footer">
      <span>🛏 <strong>
        <span data-lang="fr" class="active">Hôtel Lyubimiy</span>
        <span data-lang="en">Lyubimiy Hotel</span>
        <span data-lang="ru">Отель Любимый</span>
        <span data-lang="fa">هتل لیوبیمی</span>
      </strong> (
        <span data-lang="fr" class="active">près de l'aéroport</span>
        <span data-lang="en">near the airport</span>
        <span data-lang="ru">рядом с аэропортом</span>
        <span data-lang="fa">نزدیک فرودگاه</span>
      )</span>
      <span>4 400 ₽</span>
      <span class="payment-paid">✓ 
        <span data-lang="fr" class="active">Payé</span>
        <span data-lang="en">Paid</span>
        <span data-lang="ru">Оплачено</span>
        <span data-lang="fa">پرداخت شده</span>
      </span>
    </div>
  </div>
</article>

<!-- DAY 8 -->
<article class="day">
  <div class="day-index">
    <span class="num">08</span>
    <span class="date">20 · 05 · 2026</span>
  </div>
  <div class="day-content">
    <h3>
      <span data-lang="fr" class="active">Envol · 8 h 15</span>
      <span data-lang="en">Flight · 8:15 am</span>
      <span data-lang="ru">Вылет · 8:15</span>
      <span data-lang="fa">پرواز · ۸:۱۵</span>
    </h3>
    <div class="day-subtitle">
      <span data-lang="fr" class="active">7 h à l'aéroport · décollage à 8 h 15. Fin du carnet.</span>
      <span data-lang="en">7 am at the airport · take-off at 8:15. End of journal.</span>
      <span data-lang="ru">7:00 в аэропорту · взлёт в 8:15. Конец дневника.</span>
      <span data-lang="fa">ساعت ۷ در فرودگاه · پرواز در ۸:۱۵. پایان دفترچه.</span>
    </div>
  </div>
</article>
```

  </div>
</section>

<!-- ============================================================
     MAP
     ============================================================ -->

<section class="map-section" id="map-section">
  <div class="container">
    <div class="section-label">
      <span data-lang="fr" class="active">II · La carte</span>
      <span data-lang="en">II · The map</span>
      <span data-lang="ru">II · Карта</span>
      <span data-lang="fa">۲ · نقشه</span>
    </div>
    <h2 class="section-title">
      <span data-lang="fr" class="active">L'itinéraire <span class="italic">en un regard</span></span>
      <span data-lang="en">The route <span class="italic">at a glance</span></span>
      <span data-lang="ru">Маршрут <span class="italic">с высоты птичьего полёта</span></span>
      <span data-lang="fa">مسیر <span class="italic">در یک نگاه</span></span>
    </h2>
    <div id="map"></div>
    <p class="map-legend">
      <span data-lang="fr" class="active">Les numéros correspondent aux étapes clés du voyage. Cliquez les marqueurs pour plus d'infos.</span>
      <span data-lang="en">Numbers match key stops of the trip. Click a marker for details.</span>
      <span data-lang="ru">Цифры соответствуют ключевым остановкам. Нажмите на маркер, чтобы узнать больше.</span>
      <span data-lang="fa">شماره‌ها با توقف‌های اصلی سفر مطابقت دارند. برای جزئیات، روی نشانگرها بزنید.</span>
    </p>
  </div>
</section>

<!-- ============================================================
     BUDGET
     ============================================================ -->

<section class="budget-section" id="budget">
  <div class="container">
    <div class="section-label">
      <span data-lang="fr" class="active">III · Le budget</span>
      <span data-lang="en">III · The budget</span>
      <span data-lang="ru">III · Бюджет</span>
      <span data-lang="fa">۳ · بودجه</span>
    </div>
    <h2 class="section-title">
      <span data-lang="fr" class="active">Combien ça coûte, <span class="italic">au juste ?</span></span>
      <span data-lang="en">How much does it <span class="italic">actually cost?</span></span>
      <span data-lang="ru">Во <span class="italic">сколько это обходится</span></span>
      <span data-lang="fa">دقیقاً <span class="italic">چقدر هزینه دارد؟</span></span>
    </h2>

```
<div class="budget-grid">
  <div class="budget-card">
    <div class="budget-label">✈ 
      <span data-lang="fr" class="active">Vols</span>
      <span data-lang="en">Flights</span>
      <span data-lang="ru">Авиабилеты</span>
      <span data-lang="fa">پروازها</span>
    </div>
    <div class="budget-amount">40 800<span class="currency">₽</span></div>
  </div>
  <div class="budget-card">
    <div class="budget-label">🚗 
      <span data-lang="fr" class="active">Location voiture</span>
      <span data-lang="en">Car rental</span>
      <span data-lang="ru">Аренда авто</span>
      <span data-lang="fa">اجاره خودرو</span>
    </div>
    <div class="budget-amount">36 000<span class="currency">₽</span></div>
  </div>
  <div class="budget-card">
    <div class="budget-label">🛏 
      <span data-lang="fr" class="active">Hôtels</span>
      <span data-lang="en">Hotels</span>
      <span data-lang="ru">Отели</span>
      <span data-lang="fa">هتل‌ها</span>
    </div>
    <div class="budget-amount">52 000<span class="currency">₽</span></div>
  </div>
  <div class="budget-card">
    <div class="budget-label">⛽ 
      <span data-lang="fr" class="active">Essence &amp; extras</span>
      <span data-lang="en">Fuel &amp; extras</span>
      <span data-lang="ru">Бензин и доп.</span>
      <span data-lang="fa">سوخت و متفرقه</span>
    </div>
    <div class="budget-amount" style="color: var(--ink-faint); font-style: italic; font-size: 22px; padding-top: 10px;">
      <span data-lang="fr" class="active">à compter</span>
      <span data-lang="en">to be counted</span>
      <span data-lang="ru">подсчитать</span>
      <span data-lang="fa">قابل محاسبه</span>
    </div>
  </div>
</div>

<div class="budget-total">
  <div class="label">
    <span data-lang="fr" class="active">Total · vols + voiture + hôtels</span>
    <span data-lang="en">Total · flights + car + hotels</span>
    <span data-lang="ru">Итого · билеты + машина + отели</span>
    <span data-lang="fa">مجموع · پرواز + خودرو + هتل</span>
  </div>
  <div class="amount">128 800<span class="currency">₽</span></div>
</div>
```

  </div>
</section>

<!-- ============================================================
     RECAP
     ============================================================ -->

<section class="recap-section" id="recap">
  <div class="container">
    <div class="section-label">
      <span data-lang="fr" class="active">IV · Récap</span>
      <span data-lang="en">IV · Summary</span>
      <span data-lang="ru">IV · Сводка</span>
      <span data-lang="fa">۴ · خلاصه</span>
    </div>
    <h2 class="section-title">
      <span data-lang="fr" class="active">Tout en un <span class="italic">tableau</span></span>
      <span data-lang="en">Everything in <span class="italic">one table</span></span>
      <span data-lang="ru">Всё в одной <span class="italic">таблице</span></span>
      <span data-lang="fa">همه چیز در یک <span class="italic">جدول</span></span>
    </h2>

```
<div class="recap-wrapper">
  <table class="recap">
    <thead>
      <tr>
        <th>
          <span data-lang="fr" class="active">Jour</span>
          <span data-lang="en">Day</span>
          <span data-lang="ru">День</span>
          <span data-lang="fa">روز</span>
        </th>
        <th>
          <span data-lang="fr" class="active">Date</span>
          <span data-lang="en">Date</span>
          <span data-lang="ru">Дата</span>
          <span data-lang="fa">تاریخ</span>
        </th>
        <th>
          <span data-lang="fr" class="active">Étape / temps fort</span>
          <span data-lang="en">Stage / highlight</span>
          <span data-lang="ru">Этап / основное</span>
          <span data-lang="fa">مرحله / نقطه اوج</span>
        </th>
        <th>
          <span data-lang="fr" class="active">Km</span>
          <span data-lang="en">Km</span>
          <span data-lang="ru">Км</span>
          <span data-lang="fa">کیلومتر</span>
        </th>
        <th>
          <span data-lang="fr" class="active">Nuit</span>
          <span data-lang="en">Night</span>
          <span data-lang="ru">Ночь</span>
          <span data-lang="fa">شب</span>
        </th>
        <th>₽</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td class="day-num">01</td>
        <td>
          <span data-lang="fr" class="active">13 mai</span>
          <span data-lang="en">May 13</span>
          <span data-lang="ru">13 мая</span>
          <span data-lang="fa">۱۳ می</span>
        </td>
        <td>
          <span data-lang="fr" class="active">Arrivée · Doigt du Diable · cascade Kamishlinsky</span>
          <span data-lang="en">Arrival · Devil's Finger · Kamishlinsky waterfall</span>
          <span data-lang="ru">Прибытие · Чёртов палец · Камышлинский водопад</span>
          <span data-lang="fa">ورود · انگشت شیطان · آبشار کامیشلینسکی</span>
        </td>
        <td class="km-num">60</td><td>Loft 12</td><td class="km-num">6 880</td>
      </tr>
      <tr>
        <td class="day-num">02</td>
        <td>
          <span data-lang="fr" class="active">14 mai</span>
          <span data-lang="en">May 14</span>
          <span data-lang="ru">14 мая</span>
          <span data-lang="fa">۱۴ می</span>
        </td>
        <td>
          <span data-lang="fr" class="active">Col de Seminsky · cascade</span>
          <span data-lang="en">Seminsky Pass · waterfall</span>
          <span data-lang="ru">Семинский перевал · водопад</span>
          <span data-lang="fa">گردنه سمینسکی · آبشار</span>
        </td>
        <td class="km-num">200</td><td>Arbat</td><td class="km-num">6 500</td>
      </tr>
      <tr>
        <td class="day-num">03</td>
        <td>
          <span data-lang="fr" class="active">15 mai</span>
          <span data-lang="en">May 15</span>
          <span data-lang="ru">15 мая</span>
          <span data-lang="fa">۱۵ می</span>
        </td>
        <td>
          <span data-lang="fr" class="active">Chike-Taman · Ilgumensky · confluence Chuya/Katun</span>
          <span data-lang="en">Chike-Taman · Ilgumensky · Chuya/Katun confluence</span>
          <span data-lang="ru">Чике-Таман · Ильгуменский · слияние Чуи/Катуни</span>
          <span data-lang="fa">چیکه-تامان · ایلگومنسکی · تلاقی چویا/کاتون</span>
        </td>
        <td class="km-num">150</td><td>Green Kolobok</td><td class="km-num">5 900</td>
      </tr>
      <tr>
        <td class="day-num">04</td>
        <td>
          <span data-lang="fr" class="active">16 mai</span>
          <span data-lang="en">May 16</span>
          <span data-lang="ru">16 мая</span>
          <span data-lang="fa">۱۶ می</span>
        </td>
        <td>
          <span data-lang="fr" class="active">Trek · lac Geyser</span>
          <span data-lang="en">Trek · Geyser Lake</span>
          <span data-lang="ru">Поход · Гейзеровое озеро</span>
          <span data-lang="fa">کوهنوردی · دریاچه گیزر</span>
        </td>
        <td class="km-num">150</td><td>Green Kolobok</td><td class="km-num">5 900</td>
      </tr>
      <tr>
        <td class="day-num">05</td>
        <td>
          <span data-lang="fr" class="active">17 mai</span>
          <span data-lang="en">May 17</span>
          <span data-lang="ru">17 мая</span>
          <span data-lang="fa">۱۷ می</span>
        </td>
        <td>
          <span data-lang="fr" class="active">Retour nord — 300 km</span>
          <span data-lang="en">Back north — 300 km</span>
          <span data-lang="ru">Возвращение на север — 300 км</span>
          <span data-lang="fa">بازگشت به شمال — ۳۰۰ کیلومتر</span>
        </td>
        <td class="km-num">300</td><td>Loft 12</td><td class="km-num">6 880</td>
      </tr>
      <tr>
        <td class="day-num">06</td>
        <td>
          <span data-lang="fr" class="active">18 mai</span>
          <span data-lang="en">May 18</span>
          <span data-lang="ru">18 мая</span>
          <span data-lang="fa">۱۸ می</span>
        </td>
        <td>
          <span data-lang="fr" class="active">Rochers du Dragon · Patmos · Che-Chkysh</span>
          <span data-lang="en">Dragon Rocks · Patmos · Che-Chkysh</span>
          <span data-lang="ru">Скалы Дракона · Патмос · Че-Чкыш</span>
          <span data-lang="fa">صخره‌های اژدها · پاتموس · چه-چکیش</span>
        </td>
        <td class="km-num">135</td><td>Geometrika</td><td class="km-num">15 200</td>
      </tr>
      <tr>
        <td class="day-num">07</td>
        <td>
          <span data-lang="fr" class="active">19 mai</span>
          <span data-lang="en">May 19</span>
          <span data-lang="ru">19 мая</span>
          <span data-lang="fa">۱۹ می</span>
        </td>
        <td>
          <span data-lang="fr" class="active">Manzherok · Gorno-Altaïsk · lavage voiture</span>
          <span data-lang="en">Manzherok · Gorno-Altaysk · car wash</span>
          <span data-lang="ru">Манжерок · Горно-Алтайск · мойка</span>
          <span data-lang="fa">مانژروک · گورنو-آلتایسک · کارواش</span>
        </td>
        <td class="km-num">30</td><td>Lyubimiy</td><td class="km-num">4 400</td>
      </tr>
      <tr>
        <td class="day-num">08</td>
        <td>
          <span data-lang="fr" class="active">20 mai</span>
          <span data-lang="en">May 20</span>
          <span data-lang="ru">20 мая</span>
          <span data-lang="fa">۲۰ می</span>
        </td>
        <td>
          <span data-lang="fr" class="active">Vol 8 h 15 · retour</span>
          <span data-lang="en">Flight 8:15 · return</span>
          <span data-lang="ru">Вылет 8:15 · возвращение</span>
          <span data-lang="fa">پرواز ۸:۱۵ · بازگشت</span>
        </td>
        <td class="km-num">—</td><td>—</td><td class="km-num">—</td>
      </tr>
      <tr class="total-row">
        <td>Σ</td>
        <td colspan="2">
          <span data-lang="fr" class="active">Totaux du voyage</span>
          <span data-lang="en">Trip totals</span>
          <span data-lang="ru">Итого по поездке</span>
          <span data-lang="fa">مجموع سفر</span>
        </td>
        <td class="km-num">1 150</td>
        <td>
          <span data-lang="fr" class="active">7 nuits</span>
          <span data-lang="en">7 nights</span>
          <span data-lang="ru">7 ночей</span>
          <span data-lang="fa">۷ شب</span>
        </td>
        <td class="km-num">51 660</td>
      </tr>
    </tbody>
  </table>
</div>
```

  </div>
</section>

<!-- ============================================================
     FOOTER
     ============================================================ -->

<footer>
  <div class="footer-mark">Altaï · 13 → 20 · 05 · 2026</div>
  <div>
    <span data-lang="fr" class="active">Fait avec <span class="heart">♥</span></span>
    <span data-lang="en">Made with <span class="heart">♥</span></span>
    <span data-lang="ru">Сделано с <span class="heart">♥</span></span>
    <span data-lang="fa">ساخته شده با <span class="heart">♥</span></span>
  </div>
</footer>

<!-- ============================================================
     SCRIPTS
     ============================================================ -->

<script>
// ------------------ Language switcher ------------------
(function() {
  const toggle = document.getElementById('langToggle');
  const menu = document.getElementById('langMenu');
  const currentSpan = document.getElementById('lang-current');
  const buttons = menu.querySelectorAll('button[data-set-lang]');

  const codes = { fr: 'FR', en: 'EN', ru: 'RU', fa: 'فا' };
  const rtlLangs = ['fa'];
  let current = 'fr';

  function setLang(lang) {
    current = lang;
    document.documentElement.lang = lang;
    document.documentElement.dir = rtlLangs.includes(lang) ? 'rtl' : 'ltr';

    document.querySelectorAll('[data-lang]').forEach(el => {
      if (el.dataset.lang === lang) el.classList.add('active');
      else el.classList.remove('active');
    });

    currentSpan.textContent = codes[lang];

    buttons.forEach(btn => {
      btn.classList.toggle('active', btn.dataset.setLang === lang);
    });

    menu.classList.remove('open');
  }

  toggle.addEventListener('click', (e) => {
    e.stopPropagation();
    menu.classList.toggle('open');
  });
  document.addEventListener('click', () => menu.classList.remove('open'));

  buttons.forEach(btn => {
    btn.addEventListener('click', (e) => {
      e.stopPropagation();
      setLang(btn.dataset.setLang);
    });
  });
})();

// ------------------ Map ------------------
(function() {
  const map = L.map('map', {
    scrollWheelZoom: false,
    zoomControl: true,
  }).setView([51.0, 85.9], 7);

  L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '© OpenStreetMap',
    maxZoom: 18,
  }).addTo(map);

  const stops = [
    { n: 1, name: { fr: "Gorno-Altaïsk · arrivée", en: "Gorno-Altaysk · arrival", ru: "Горно-Алтайск · прибытие", fa: "گورنو-آلتایسک · ورود" }, coords: [51.9586, 85.9601] },
    { n: 1, name: { fr: "Chertov Palets · Doigt du Diable", en: "Chertov Palets · Devil's Finger", ru: "Чёртов палец", fa: "انگشت شیطان" }, coords: [51.7956, 85.7350] },
    { n: 1, name: { fr: "Cascade Kamishlinsky", en: "Kamishlinsky waterfall", ru: "Камышлинский водопад", fa: "آبشار کامیشلینسکی" }, coords: [51.7000, 85.7500] },
    { n: 2, name: { fr: "Col de Seminsky", en: "Seminsky Pass", ru: "Семинский перевал", fa: "گردنه سمینسکی" }, coords: [51.0333, 85.6000] },
    { n: 2, name: { fr: "Arbat hôtel", en: "Arbat hotel", ru: "Отель Арбат", fa: "هتل آرباط" }, coords: [50.7500, 86.2000] },
    { n: 3, name: { fr: "Col de Chike-Taman", en: "Chike-Taman Pass", ru: "Перевал Чике-Таман", fa: "گردنه چیکه-تامان" }, coords: [50.6394, 86.3181] },
    { n: 3, name: { fr: "Confluence Chuya + Katun", en: "Chuya + Katun confluence", ru: "Слияние Чуи и Катуни", fa: "تلاقی چویا و کاتون" }, coords: [50.4067, 86.6786] },
    { n: 3, name: { fr: "Cascade Shirlak", en: "Shirlak waterfall", ru: "Водопад Ширлак", fa: "آبشار شیرلاک" }, coords: [50.3667, 87.3000] },
    { n: 3, name: { fr: "Green Kolobok", en: "Green Kolobok", ru: "Зелёный Колобок", fa: "گرین کولوبوک" }, coords: [50.2000, 87.5500] },
    { n: 4, name: { fr: "Lac Geyser", en: "Geyser Lake", ru: "Гейзеровое озеро", fa: "دریاچه گیزر" }, coords: [50.2833, 87.6500] },
    { n: 6, name: { fr: "Île de Patmos (Chemal)", en: "Patmos Island (Chemal)", ru: "Остров Патмос (Чемал)", fa: "جزیره پاتموس (چمال)" }, coords: [51.4097, 86.0100] },
    { n: 6, name: { fr: "Cascade Che-Chkysh", en: "Che-Chkysh waterfall", ru: "Водопад Че-Чкыш", fa: "آبشار چه-چکیش" }, coords: [51.3500, 86.1000] },
    { n: 6, name: { fr: "Manzherok", en: "Manzherok", ru: "Манжерок", fa: "مانژروک" }, coords: [51.8256, 85.7897] },
    { n: 7, name: { fr: "Gorno-Altaïsk · hôtel Lyubimiy", en: "Gorno-Altaysk · Lyubimiy hotel", ru: "Горно-Алтайск · отель Любимый", fa: "گورنو-آلتایسک · هتل لیوبیمی" }, coords: [51.9600, 85.9650] },
  ];

  function makeIcon(n) {
    return L.divIcon({
      className: 'custom-marker',
      html: `<div style="
        width: 30px; height: 30px;
        background: #b03a2e;
        color: #f1e8d6;
        border: 2px solid #f1e8d6;
        border-radius: 50%;
        display: flex; align-items: center; justify-content: center;
        font-family: Fraunces, serif;
        font-weight: 600;
        font-size: 14px;
        box-shadow: 0 3px 8px rgba(42,31,20,.4);
      ">${n}</div>`,
      iconSize: [30, 30],
      iconAnchor: [15, 15],
    });
  }

  const dayLabels = {
    fr: 'Jour', en: 'Day', ru: 'День', fa: 'روز'
  };

  const latlngs = [];
  const markers = [];
  stops.forEach(stop => {
    const marker = L.marker(stop.coords, { icon: makeIcon(stop.n) }).addTo(map);
    marker._stopData = stop;
    marker.bindPopup(buildPopup(stop, 'fr'));
    markers.push(marker);
    latlngs.push(stop.coords);
  });

  function buildPopup(stop, lang) {
    return `
      <div style="font-family: ${lang === 'fa' ? 'Vazirmatn, sans-serif' : 'Fraunces, serif'}; font-size: 15px; ${lang === 'fa' ? 'direction: rtl; text-align: right;' : ''}">
        <div style="font-size:11px;text-transform:uppercase;letter-spacing:.18em;color:#8a7557;margin-bottom:4px;">${dayLabels[lang]} ${stop.n}</div>
        <strong style="font-weight:500;">${stop.name[lang]}</strong>
      </div>`;
  }

  // Update popups when language changes
  const observer = new MutationObserver(() => {
    const lang = document.documentElement.lang || 'fr';
    markers.forEach(m => m.setPopupContent(buildPopup(m._stopData, lang)));
  });
  observer.observe(document.documentElement, { attributes: true, attributeFilter: ['lang'] });

  L.polyline(latlngs, {
    color: '#b03a2e',
    weight: 2,
    opacity: 0.55,
    dashArray: '6, 8',
  }).addTo(map);

  map.fitBounds(L.latLngBounds(latlngs).pad(0.15));
})();
</script>

</body>
</html>
