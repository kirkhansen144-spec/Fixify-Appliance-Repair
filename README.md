<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Fixify Appliance Repair | Newburgh, Chandler &amp; Evansville, IN</title>
<meta name="description" content="Fixify Appliance Repair fixes refrigerators, washers, dryers, dishwashers, ovens and more across Newburgh, Chandler, and Evansville, Indiana. Flat $100 diagnosis, clear communication, on-time arrival, spotless cleanup.">
<link rel="icon" type="image/png" href="assets/fixify-badge.png">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Oswald:wght@500;600;700&family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
<style>
  :root{
    --ink:#21232A;
    --ink-soft:#3B3E46;
    --orange:#E8590B;
    --orange-dark:#C94D08;
    --slate:#6C727E;
    --steel:#F2F4F6;
    --steel-line:#E1E5E9;
    --white:#FFFFFF;
    --deep:#1B1D22;
    --deep-line:#33363E;
    --radius:10px;
    --wrap:1120px;
    --font-display: 'Oswald', sans-serif;
    --font-body: 'Inter', sans-serif;
  }

  *,*::before,*::after{ box-sizing:border-box; }
  html{ scroll-behavior:smooth; }
  body{
    margin:0;
    font-family:var(--font-body);
    color:var(--ink);
    background:var(--white);
    line-height:1.55;
    -webkit-font-smoothing:antialiased;
  }
  img{ max-width:100%; display:block; }
  a{ color:inherit; }
  h1,h2,h3{
    font-family:var(--font-display);
    font-weight:600;
    line-height:1.12;
    margin:0;
    letter-spacing:0.2px;
  }
  p{ margin:0; }
  ul{ margin:0; padding:0; list-style:none; }
  button{ font-family:inherit; }

  .wrap{
    max-width:var(--wrap);
    margin:0 auto;
    padding:0 24px;
  }

  :focus-visible{
    outline:3px solid var(--orange);
    outline-offset:2px;
  }

  @media (prefers-reduced-motion: reduce){
    *{ animation:none !important; transition:none !important; scroll-behavior:auto !important; }
  }

  /* ---------- buttons ---------- */
  .btn{
    display:inline-flex;
    align-items:center;
    justify-content:center;
    gap:8px;
    padding:14px 26px;
    border-radius:var(--radius);
    font-weight:600;
    font-size:0.98rem;
    text-decoration:none;
    border:2px solid transparent;
    cursor:pointer;
    transition:background-color .15s ease, border-color .15s ease, transform .15s ease, color .15s ease;
    white-space:nowrap;
  }
  .btn-primary{
    background:var(--orange-dark);
    color:var(--white);
  }
  .btn-primary:hover{ background:#a8420a; transform:translateY(-1px); }
  .btn-ghost{
    background:transparent;
    color:var(--ink);
    border-color:var(--ink);
  }
  .btn-ghost:hover{ background:var(--ink); color:var(--white); }
  .btn-ghost-light{
    background:transparent;
    color:var(--white);
    border-color:rgba(255,255,255,0.5);
  }
  .btn-ghost-light:hover{ background:rgba(255,255,255,0.12); border-color:var(--white); }
  .btn-block{ width:100%; }

  /* ---------- header ---------- */
  .site-header{
    position:sticky;
    top:0;
    z-index:50;
    background:rgba(255,255,255,0.94);
    backdrop-filter:saturate(180%) blur(8px);
    border-bottom:1px solid var(--steel-line);
  }
  .nav{
    display:flex;
    align-items:center;
    justify-content:space-between;
    padding:14px 0;
    gap:16px;
  }
  .nav-logo img{ height:38px; width:auto; }
  .nav-logo{ display:flex; align-items:center; }
  .nav-links{
    display:none;
    align-items:center;
    gap:32px;
    font-weight:500;
    font-size:0.95rem;
  }
  .nav-links a{ text-decoration:none; color:var(--ink-soft); }
  .nav-links a:hover{ color:var(--orange); }
  .nav-actions{ display:flex; align-items:center; gap:14px; }
  .nav-phone{
    display:none;
    font-weight:600;
    text-decoration:none;
    color:var(--ink);
    font-size:0.95rem;
  }
  .nav-toggle{
    display:inline-flex;
    align-items:center;
    justify-content:center;
    width:42px;
    height:42px;
    border-radius:8px;
    border:1px solid var(--steel-line);
    background:var(--white);
  }
  .nav-toggle svg{ width:20px; height:20px; }

  .mobile-menu{
    display:none;
    flex-direction:column;
    gap:2px;
    padding:8px 0 18px;
    border-top:1px solid var(--steel-line);
  }
  .mobile-menu.open{ display:flex; }
  .mobile-menu a{
    padding:12px 4px;
    text-decoration:none;
    color:var(--ink-soft);
    font-weight:500;
    border-bottom:1px solid var(--steel-line);
  }
  .mobile-menu .btn{ margin-top:12px; }

  @media (min-width:900px){
    .nav-links{ display:flex; }
    .nav-phone{ display:inline-block; }
    .nav-toggle{ display:none; }
  }

  /* ---------- hero ---------- */
  .hero{
    padding:64px 0 56px;
    background:var(--steel);
    overflow:hidden;
  }
  .hero .wrap{
    display:grid;
    gap:40px;
    align-items:center;
  }
  .hero-locality{
    display:inline-flex;
    align-items:center;
    gap:8px;
    font-size:0.85rem;
    font-weight:600;
    color:var(--orange-dark);
    background:rgba(232,89,11,0.1);
    padding:7px 14px;
    border-radius:999px;
    margin-bottom:20px;
  }
  .hero-locality svg{ width:14px; height:14px; flex-shrink:0; }
  .hero h1{
    font-size:2.5rem;
    color:var(--ink);
    max-width:14ch;
  }
  .hero-sub{
    margin-top:20px;
    font-size:1.08rem;
    color:var(--ink-soft);
    max-width:46ch;
  }
  .hero-cta{
    display:flex;
    flex-wrap:wrap;
    gap:14px;
    margin-top:30px;
  }
  .hero-art{
    display:flex;
    justify-content:center;
    animation:settle-in 0.7s ease-out both;
  }
  .hero-art img{ width:min(280px, 62vw); filter:drop-shadow(0 18px 30px rgba(33,35,42,0.22)); }

  @keyframes settle-in{
    from{ opacity:0; transform:translateY(14px) scale(0.97); }
    to{ opacity:1; transform:translateY(0) scale(1); }
  }

  @media (min-width:800px){
    .hero{ padding:96px 0 84px; }
    .hero .wrap{ grid-template-columns:1.15fr 0.85fr; }
    .hero h1{ font-size:3.4rem; max-width:12ch; }
    .hero-art img{ width:min(360px, 100%); }
  }

  /* ---------- section heading pattern ---------- */
  .section-head{ max-width:56ch; margin-bottom:40px; }
  .section-head h2{ font-size:2rem; color:var(--ink); }
  .section-head p{ margin-top:12px; color:var(--slate); font-size:1.02rem; }
  .section-head.center{ margin-left:auto; margin-right:auto; text-align:center; }

  section{ padding:72px 0; }

  /* ---------- trust strip ---------- */
  .trust{ background:var(--white); }
  .trust-grid{
    display:grid;
    gap:36px;
  }
  .trust-item{
    display:flex;
    gap:16px;
  }
  .trust-icon{
    flex-shrink:0;
    width:46px;
    height:46px;
    border-radius:9px;
    background:var(--steel);
    display:flex;
    align-items:center;
    justify-content:center;
  }
  .trust-icon svg{ width:24px; height:24px; stroke:var(--orange-dark); }
  .trust-item h3{ font-size:1.08rem; color:var(--ink); }
  .trust-item p{ margin-top:6px; color:var(--slate); font-size:0.96rem; }

  @media (min-width:800px){
    .trust-grid{ grid-template-columns:repeat(3,1fr); }
    .trust-item{ padding-right:12px; border-left:1px solid var(--steel-line); padding-left:24px; }
    .trust-item:first-child{ border-left:none; padding-left:0; }
  }

  /* ---------- services ---------- */
  .services{ background:var(--steel); }
  .service-grid{
    display:grid;
    grid-template-columns:repeat(2,1fr);
    gap:14px;
  }
  .service-card{
    background:var(--white);
    border:1px solid var(--steel-line);
    border-radius:var(--radius);
    padding:20px 16px;
    display:flex;
    flex-direction:column;
    align-items:flex-start;
    gap:12px;
  }
  .service-card svg{ width:34px; height:34px; }
  .service-card span{ font-weight:600; font-size:0.95rem; }
  .services-note{
    margin-top:28px;
    color:var(--slate);
    font-size:0.98rem;
    max-width:60ch;
  }
  .services-note strong{ color:var(--ink); }

  @media (min-width:600px){
    .service-grid{ grid-template-columns:repeat(4,1fr); }
  }

  /* ---------- pricing ---------- */
  .pricing{ background:var(--white); }
  .steps{
    display:grid;
    gap:16px;
    position:relative;
  }
  .step{
    display:flex;
    gap:18px;
    background:var(--steel);
    border-radius:var(--radius);
    padding:26px 24px;
  }
  .step-num{
    flex-shrink:0;
    width:38px;
    height:38px;
    border-radius:50%;
    background:var(--ink);
    color:var(--white);
    font-family:var(--font-display);
    font-weight:600;
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:1.05rem;
  }
  .step.is-repair .step-num{ background:var(--orange-dark); }
  .step h3{ font-size:1.15rem; color:var(--ink); }
  .step p{ margin-top:6px; color:var(--slate); font-size:0.97rem; }
  .step .price{ color:var(--orange-dark); font-weight:700; }

  .price-note{
    margin-top:22px;
    padding:16px 20px;
    border:1px dashed var(--steel-line);
    border-radius:var(--radius);
    color:var(--ink-soft);
    font-size:0.95rem;
  }

  @media (min-width:800px){
    .steps{ grid-template-columns:1fr 1fr; }
  }

  /* ---------- areas ---------- */
  .areas{ background:var(--steel); text-align:center; }
  .area-chips{
    display:flex;
    flex-wrap:wrap;
    gap:12px;
    justify-content:center;
    margin-top:8px;
  }
  .area-chip{
    display:inline-flex;
    align-items:center;
    gap:8px;
    background:var(--white);
    border:1px solid var(--steel-line);
    border-radius:999px;
    padding:12px 22px;
    font-weight:600;
    font-size:0.98rem;
  }
  .area-chip svg{ width:16px; height:16px; stroke:var(--orange-dark); flex-shrink:0; }

  /* ---------- CTA ---------- */
  .cta{
    background:var(--deep);
    color:var(--white);
  }
  .cta-inner{
    display:flex;
    flex-direction:column;
    gap:28px;
    align-items:flex-start;
  }
  .cta h2{ color:var(--white); font-size:2rem; max-width:16ch; }
  .cta p{ color:#B7BAC2; margin-top:14px; max-width:48ch; font-size:1.02rem; }
  .cta-details{
    display:flex;
    flex-wrap:wrap;
    gap:28px;
    margin-top:26px;
  }
  .cta-detail{ font-size:0.95rem; }
  .cta-detail span{ display:block; color:#9AA0AB; margin-bottom:4px; }
  .cta-detail a, .cta-detail strong{ font-size:1.08rem; font-weight:600; color:var(--white); text-decoration:none; }
  .cta-buttons{ display:flex; flex-wrap:wrap; gap:14px; margin-top:8px; }

  @media (min-width:800px){
    .cta-inner{ flex-direction:row; justify-content:space-between; align-items:center; }
    .cta-buttons{ flex-direction:column; align-items:stretch; min-width:220px; }
  }

  /* ---------- footer ---------- */
  .site-footer{
    background:var(--ink);
    color:#C7C9CF;
    padding:48px 0 28px;
  }
  .footer-top{
    display:flex;
    flex-direction:column;
    gap:28px;
    padding-bottom:32px;
    border-bottom:1px solid var(--deep-line);
  }
  .footer-logo img{ height:34px; }
  .footer-tagline{ margin-top:14px; max-width:38ch; font-size:0.94rem; color:#9EA1AA; }
  .footer-links{ display:flex; flex-wrap:wrap; gap:22px; font-size:0.92rem; }
  .footer-links a{ text-decoration:none; color:#C7C9CF; }
  .footer-links a:hover{ color:var(--orange); }
  .footer-bottom{
    padding-top:22px;
    display:flex;
    flex-direction:column;
    gap:10px;
    font-size:0.85rem;
    color:#8B8E97;
  }

  @media (min-width:800px){
    .footer-top{ flex-direction:row; justify-content:space-between; align-items:flex-start; }
    .footer-bottom{ flex-direction:row; justify-content:space-between; }
  }
</style>
</head>
<body>

<header class="site-header">
  <div class="wrap">
    <nav class="nav">
      <a href="#top" class="nav-logo" aria-label="Fixify Appliance Repair home">
        <img src="assets/fixify-lockup-light.png" alt="Fixify Appliance Repair">
      </a>
      <ul class="nav-links">
        <li><a href="#services">Services</a></li>
        <li><a href="#pricing">Pricing</a></li>
        <li><a href="#areas">Areas We Serve</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
      <div class="nav-actions">
        <a class="nav-phone" href="tel:+12704850836">(270) 485-0836</a>
        <button class="nav-toggle" id="nav-toggle" aria-label="Open menu" aria-expanded="false" aria-controls="mobile-menu">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round"><line x1="3" y1="6" x2="21" y2="6"/><line x1="3" y1="12" x2="21" y2="12"/><line x1="3" y1="18" x2="21" y2="18"/></svg>
        </button>
      </div>
    </nav>
    <div class="mobile-menu" id="mobile-menu">
      <a href="#services">Services</a>
      <a href="#pricing">Pricing</a>
      <a href="#areas">Areas We Serve</a>
      <a href="#contact">Contact</a>
      <a class="btn btn-primary btn-block" href="tel:+12704850836">Call (270) 485-0836</a>
    </div>
  </div>
</header>

<main id="top">

  <!-- HERO -->
  <section class="hero">
    <div class="wrap">
      <div>
        <span class="hero-locality">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 21s-7-6.1-7-11.5A7 7 0 0 1 19 9.5C19 14.9 12 21 12 21z"/><circle cx="12" cy="9.5" r="2.4"/></svg>
          Serving Newburgh, Chandler &amp; Evansville, IN
        </span>
        <h1>Appliance repair without the runaround.</h1>
        <p class="hero-sub">Fixify keeps your refrigerator, washer, dryer, and other major appliances running — with straight answers from the first call to the final wipe-down, and a flat $100 diagnosis that goes straight toward your repair.</p>
        <div class="hero-cta">
          <a href="tel:+12704850836" class="btn btn-primary">Call (270) 485-0836</a>
          <a href="#pricing" class="btn btn-ghost">See how pricing works</a>
        </div>
      </div>
      <div class="hero-art">
        <img src="assets/fixify-badge.png" alt="Fixify Appliance Repair badge logo">
      </div>
    </div>
  </section>

  <!-- TRUST -->
  <section class="trust">
    <div class="wrap trust-grid">
      <div class="trust-item">
        <div class="trust-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
        </div>
        <div>
          <h3>Clear communication</h3>
          <p>You'll know what's wrong, what it costs, and when we're arriving — no guessing games.</p>
        </div>
      </div>
      <div class="trust-item">
        <div class="trust-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="9"/><path d="M12 7v5l3.5 2"/></svg>
        </div>
        <div>
          <h3>On time, every time</h3>
          <p>We give you a real arrival window and show up in it, so your whole day isn't on hold.</p>
        </div>
      </div>
      <div class="trust-item">
        <div class="trust-icon">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4 20l6-6"/><path d="M13.5 4.5c1.5-1.5 4-1.5 5.5 0s1.5 4 0 5.5L9 20l-5-5z"/><path d="M14.5 7.5l2 2"/></svg>
        </div>
        <div>
          <h3>Leaves it spotless</h3>
          <p>We clean up our work area before we leave. Your kitchen shouldn't look like a job site.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- SERVICES -->
  <section class="services" id="services">
    <div class="wrap">
      <div class="section-head">
        <h2>What we repair</h2>
        <p>Most major appliances, most major brands — in your kitchen, laundry room, or wherever they've decided to break.</p>
      </div>
      <div class="service-grid">
        <div class="service-card">
          <svg viewBox="0 0 48 48" fill="none" stroke="#21232A" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="12" y="4" width="24" height="40" rx="4"/><line x1="12" y1="20" x2="36" y2="20"/><circle cx="30" cy="12" r="1.6" fill="#E8590B" stroke="none"/><circle cx="30" cy="28" r="1.6" fill="#E8590B" stroke="none"/></svg>
          <span>Refrigerators</span>
        </div>
        <div class="service-card">
          <svg viewBox="0 0 48 48" fill="none" stroke="#21232A" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="8" y="6" width="32" height="36" rx="5"/><circle cx="24" cy="26" r="9"/><circle cx="15" cy="13" r="1.6" fill="#E8590B" stroke="none"/><circle cx="22" cy="13" r="1.4"/></svg>
          <span>Washers</span>
        </div>
        <div class="service-card">
          <svg viewBox="0 0 48 48" fill="none" stroke="#21232A" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="8" y="6" width="32" height="36" rx="5"/><circle cx="24" cy="27" r="8"/><path d="M20 24a4 4 0 0 0 6 5" /><circle cx="15" cy="13" r="1.6" fill="#E8590B" stroke="none"/><circle cx="22" cy="13" r="1.4"/></svg>
          <span>Dryers</span>
        </div>
        <div class="service-card">
          <svg viewBox="0 0 48 48" fill="none" stroke="#21232A" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="9" y="4" width="30" height="40" rx="4"/><line x1="9" y1="14" x2="39" y2="14"/><rect x="14" y="21" width="20" height="16" rx="2"/><circle cx="33" cy="9" r="1.6" fill="#E8590B" stroke="none"/></svg>
          <span>Dishwashers</span>
        </div>
        <div class="service-card">
          <svg viewBox="0 0 48 48" fill="none" stroke="#21232A" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="6" y="6" width="36" height="36" rx="4"/><rect x="11" y="20" width="26" height="16" rx="2"/><circle cx="13" cy="13" r="1.8"/><circle cx="20" cy="13" r="1.8"/><circle cx="27" cy="13" r="1.8" fill="#E8590B" stroke="none"/><circle cx="34" cy="13" r="1.8"/></svg>
          <span>Ovens &amp; Ranges</span>
        </div>
        <div class="service-card">
          <svg viewBox="0 0 48 48" fill="none" stroke="#21232A" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="4" y="14" width="40" height="22" rx="4"/><circle cx="15" cy="25" r="4.5"/><circle cx="33" cy="25" r="4.5" stroke="#E8590B"/></svg>
          <span>Cooktops</span>
        </div>
        <div class="service-card">
          <svg viewBox="0 0 48 48" fill="none" stroke="#21232A" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M24 4v15"/><path d="M17 12l7 7 7-7"/><rect x="9" y="24" width="30" height="16" rx="3"/><line x1="15" y1="32" x2="26" y2="32"/><circle cx="32" cy="32" r="1.6" fill="#E8590B" stroke="none"/></svg>
          <span>Appliance Installation</span>
        </div>
      </div>
      <p class="services-note"><strong>Don't see your appliance listed?</strong> Give us a call — if it runs on electricity or gas in your kitchen or laundry room, there's a good chance we can fix it.</p>
    </div>
  </section>

  <!-- PRICING -->
  <section class="pricing" id="pricing">
    <div class="wrap">
      <div class="section-head">
        <h2>Simple, honest pricing</h2>
        <p>One flat fee to find the problem. If you move forward with the repair, it comes right off the total.</p>
      </div>
      <div class="steps">
        <div class="step">
          <div class="step-num">1</div>
          <div>
            <h3>Diagnosis — <span class="price">$100 flat</span></h3>
            <p>We inspect the appliance, track down the issue, and give you a straightforward repair quote before we do anything else.</p>
          </div>
        </div>
        <div class="step is-repair">
          <div class="step-num">2</div>
          <div>
            <h3>Repair — <span class="price">fee applied to total</span></h3>
            <p>Approve the quote and we get to work right away. Your $100 diagnosis fee is credited toward the final bill.</p>
          </div>
        </div>
      </div>
      <p class="price-note">No repair, no pressure — if you decide not to move forward, you only ever pay the $100 diagnosis fee.</p>
    </div>
  </section>

  <!-- AREAS -->
  <section class="areas" id="areas">
    <div class="wrap">
      <div class="section-head center">
        <h2>Proudly serving three communities</h2>
        <p>Local, dependable appliance repair across the tri-area.</p>
      </div>
      <div class="area-chips">
        <span class="area-chip">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 21s-7-6.1-7-11.5A7 7 0 0 1 19 9.5C19 14.9 12 21 12 21z"/><circle cx="12" cy="9.5" r="2.4"/></svg>
          Newburgh, IN
        </span>
        <span class="area-chip">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 21s-7-6.1-7-11.5A7 7 0 0 1 19 9.5C19 14.9 12 21 12 21z"/><circle cx="12" cy="9.5" r="2.4"/></svg>
          Chandler, IN
        </span>
        <span class="area-chip">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 21s-7-6.1-7-11.5A7 7 0 0 1 19 9.5C19 14.9 12 21 12 21z"/><circle cx="12" cy="9.5" r="2.4"/></svg>
          Evansville, IN
        </span>
      </div>
    </div>
  </section>

  <!-- CTA -->
  <section class="cta" id="contact">
    <div class="wrap cta-inner">
      <div>
        <h2>Ready when your appliance isn't.</h2>
        <p>Call or text to get on the schedule. We'll walk you through next steps and give you a real arrival window — no runaround.</p>
        <div class="cta-details">
          <div class="cta-detail">
            <span>Call or text</span>
            <a href="tel:+12704850836">(270) 485-0836</a>
          </div>
          <div class="cta-detail">
            <span>Hours</span>
            <strong>Mon–Fri, 9am–5pm</strong>
          </div>
        </div>
      </div>
      <div class="cta-buttons">
        <a href="tel:+12704850836" class="btn btn-primary">Call Fixify now</a>
        <a href="sms:+12704850836" class="btn btn-ghost-light">Text us instead</a>
      </div>
    </div>
  </section>

</main>

<footer class="site-footer">
  <div class="wrap">
    <div class="footer-top">
      <div>
        <a href="#top" class="footer-logo" aria-label="Fixify Appliance Repair home">
          <img src="assets/fixify-lockup-dark.png" alt="Fixify Appliance Repair">
        </a>
        <p class="footer-tagline">Appliance repair for Newburgh, Chandler, and Evansville, Indiana — professional communication, on-time arrival, spotless cleanup.</p>
      </div>
      <ul class="footer-links">
        <li><a href="#services">Services</a></li>
        <li><a href="#pricing">Pricing</a></li>
        <li><a href="#areas">Areas We Serve</a></li>
        <li><a href="tel:+12704850836">(270) 485-0836</a></li>
      </ul>
    </div>
    <div class="footer-bottom">
      <span>&copy; <span id="year">2026</span> Fixify Appliance Repair. All rights reserved.</span>
      <span>Newburgh &middot; Chandler &middot; Evansville, IN</span>
    </div>
  </div>
</footer>

<script>
  var toggle = document.getElementById('nav-toggle');
  var menu = document.getElementById('mobile-menu');
  toggle.addEventListener('click', function(){
    var isOpen = menu.classList.toggle('open');
    toggle.setAttribute('aria-expanded', isOpen ? 'true' : 'false');
  });
  menu.querySelectorAll('a').forEach(function(link){
    link.addEventListener('click', function(){
      menu.classList.remove('open');
      toggle.setAttribute('aria-expanded', 'false');
    });
  });
  document.getElementById('year').textContent = new Date().getFullYear();
</script>

</body>
</html>
