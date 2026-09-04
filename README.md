<!DOCTYPE html>
<html lang="fa-AF" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<meta name="description" content="مرکز آموزشی و توانبخشی نگین؛ آموزش، توانبخشی و حمایت از کودکان دارای معلولیت و کودکان نورودیورجنت در افغانستان.">
<meta name="keywords" content="مرکز آموزشی نگین, توانبخشی کودکان, اوتیسم, ADHD, فیزیوتراپی, کاردرمانی, گفتاردرمانی, افغانستان, کابل">
<meta name="author" content="مرکز آموزشی و توانبخشی نگین">

<title>مرکز آموزشی و توانبخشی نگین | هر کودک یک نگین</title>

<style>
/* =========================================================
   NEGIN EDUCATIONAL & REHABILITATION CENTER
   GitHub Pages — Single File Complete Website
========================================================= */

@import url('https://fonts.googleapis.com/css2?family=Tajawal:wght@400;500;600;700;800;900&display=swap');

:root {
    --primary:#075985;
    --primary-dark:#043b4d;
    --primary-light:#0ea5e9;
    --gold:#ffc800;
    --gold-dark:#c99d00;
    --gold-light:#ffe066;
    --green:#15803d;
    --green-light:#22c55e;
    --red:#dc2626;
    --orange:#ea580c;
    --purple:#7c3aed;
    --background:#f7fafc;
    --surface:#ffffff;
    --surface-soft:#eef5f8;
    --surface-hover:#e2edf2;
    --text:#172033;
    --text-soft:#475569;
    --text-light:#64748b;
    --border:#d8e1e8;
    --shadow:0 10px 35px rgba(15,23,42,.08);
    --shadow-lg:0 20px 60px rgba(15,23,42,.14);
    --radius:22px;
    --header-height:85px;
}

body.dark {
    --background:#081419;
    --surface:#102129;
    --surface-soft:#142b34;
    --surface-hover:#1a3340;
    --text:#f1f5f9;
    --text-soft:#cbd5e1;
    --text-light:#a7b6c0;
    --border:#29404a;
    --shadow:0 10px 35px rgba(0,0,0,.30);
    --shadow-lg:0 20px 60px rgba(0,0,0,.45);
}

body.high-contrast {
    --primary:#000;
    --primary-dark:#000;
    --primary-light:#000;
    --gold:#ffff00;
    --background:#fff;
    --surface:#fff;
    --surface-soft:#fff;
    --text:#000;
    --text-soft:#000;
    --text-light:#000;
    --border:#000;
    --shadow:none;
}

* { margin:0; padding:0; box-sizing:border-box; }
html { scroll-behavior:smooth; }
body {
    font-family:"Tajawal","Vazirmatn","Segoe UI",Arial,sans-serif;
    background:var(--background);
    color:var(--text);
    line-height:1.9;
    transition: background .3s ease, color .3s ease;
    overflow-x:hidden;
}
a { color:inherit; text-decoration:none; }
button, input, textarea, select { font-family:inherit; }
img { max-width:100%; display:block; }
.container { width:min(1180px,calc(100% - 32px)); margin:auto; }

.skip-link {
    position:fixed; top:-100px; right:20px;
    background:#000; color:#fff;
    padding:10px 18px; border-radius:10px; z-index:9999;
}
.skip-link:focus { top:20px; }
:focus-visible { outline:3px solid var(--gold); outline-offset:3px; }

.topbar { background:var(--primary-dark); color:#fff; font-size:13px; padding:7px 0; }
.topbar-inner { display:flex; justify-content:space-between; align-items:center; gap:15px; }
.topbar-contact { display:flex; gap:18px; flex-wrap:wrap; }
.topbar a:hover { color:var(--gold); }

.main-header {
    height:var(--header-height); position:sticky; top:0; z-index:1000;
    background:rgba(255,255,255,.94); backdrop-filter:blur(18px);
    border-bottom:1px solid var(--border); box-shadow:0 5px 25px rgba(0,0,0,.05);
}
.dark .main-header { background:rgba(16,33,41,.94); }
.header-inner { height:100%; display:grid; grid-template-columns:80px 1fr 80px; align-items:center; gap:10px; }
.menu-side { display:flex; justify-content:flex-start; }
.header-actions { display:flex; justify-content:flex-end; }

.icon-btn {
    width:48px; height:48px; border:1px solid var(--border); border-radius:15px;
    background:var(--surface); color:var(--primary); display:flex; align-items:center;
    justify-content:center; cursor:pointer; transition:.25s; box-shadow:var(--shadow);
}
.icon-btn:hover { transform:translateY(-2px); background:var(--primary); color:#fff; }
.icon-btn svg { width:23px; height:23px; fill:none; stroke:currentColor; stroke-width:2; stroke-linecap:round; stroke-linejoin:round; }

/* BRAND & LOGO STYLES */
.brand { text-align:center; display:flex; justify-content:center; align-items:center; }
.brand-logo-wrapper { display:flex; align-items:center; gap:12px; }
.brand-logo { height:68px; width:auto; max-width:100%; object-fit:contain; border-radius:12px; }

.side-menu {
    position:fixed; top:0; left:0; width:min(370px,88vw); height:100vh;
    background:var(--surface); z-index:2000; transform:translateX(-105%);
    transition:transform .35s ease; box-shadow:15px 0 50px rgba(0,0,0,.2); overflow-y:auto;
}
.side-menu.open { transform:translateX(0); }
.menu-head {
    padding:22px; background:linear-gradient(135deg, var(--primary-dark), var(--primary));
    color:#fff; display:flex; justify-content:space-between; align-items:center;
}
.menu-head-title { font-size:18px; font-weight:900; }
.menu-close { background:rgba(255,255,255,.15); color:#fff; border:0; width:42px; height:42px; border-radius:12px; cursor:pointer; font-size:25px; }
.menu-list { list-style:none; padding:15px; }
.menu-list li { margin-bottom:5px; }
.menu-list a { display:flex; align-items:center; gap:12px; padding:12px 15px; border-radius:12px; color:var(--text); font-weight:600; transition:.2s; }
.menu-list a:hover { background:var(--surface-soft); color:var(--primary); transform:translateX(-3px); }
.menu-icon { font-size:20px; width:28px; text-align:center; }
.menu-overlay { position:fixed; inset:0; background:rgba(0,0,0,.55); z-index:1900; opacity:0; visibility:hidden; transition:.3s; }
.menu-overlay.show { opacity:1; visibility:visible; }

.hero { min-height:640px; position:relative; overflow:hidden; background:#062d3a; }
.hero-slider { position:absolute; inset:0; }
.hero-slide { position:absolute; inset:0; opacity:0; transition:opacity 1s ease; background-size:cover; background-position:center; }
.hero-slide.active { opacity:1; }
.hero-slide::after { content:""; position:absolute; inset:0; background:linear-gradient(90deg, rgba(3,28,37,.92), rgba(3,28,37,.68), rgba(3,28,37,.30)); }
.hero-slide:nth-child(1) { background-image:url("https://images.unsplash.com/photo-1542810634-71277d95dcbb?auto=format&fit=crop&w=1800&q=85"); }
.hero-slide:nth-child(2) { background-image:url("https://images.unsplash.com/photo-1504159506876-f8338247a14a?auto=format&fit=crop&w=1800&q=85"); }
.hero-slide:nth-child(3) { background-image:url("https://images.unsplash.com/photo-1472162072942-cd5147eb3902?auto=format&fit=crop&w=1800&q=85"); }
.hero-slide:nth-child(4) { background-image:url("https://images.unsplash.com/photo-1503454537195-1dcabb73ffb9?auto=format&fit=crop&w=1800&q=85"); }

.hero-content { position:relative; z-index:5; min-height:640px; display:flex; align-items:center; }
.hero-text { width:min(760px,100%); color:#fff; padding:50px 0; }
.hero-kicker { display:inline-flex; padding:8px 15px; border:1px solid rgba(255,255,255,.3); border-radius:30px; background:rgba(255,255,255,.1); backdrop-filter:blur(8px); font-size:14px; margin-bottom:20px; }
.hero-title { font-size:clamp(34px,6vw,68px); line-height:1.25; font-weight:900; margin-bottom:18px; }
.hero-title span { color:var(--gold); }
.hero-subtitle { font-size:clamp(17px,2.5vw,23px); line-height:1.9; color:#f1f5f9; max-width:700px; margin-bottom:28px; }
.hero-buttons { display:flex; gap:12px; flex-wrap:wrap; }

.btn { display:inline-flex; align-items:center; justify-content:center; gap:8px; min-height:48px; padding:10px 22px; border-radius:14px; border:1px solid transparent; font-weight:800; cursor:pointer; transition:.25s; }
.btn-gold { background:var(--gold); color:#111; }
.btn-gold:hover { background:var(--gold-light); transform:translateY(-2px); }
.btn-outline { border-color:rgba(255,255,255,.5); background:rgba(255,255,255,.08); color:#fff; backdrop-filter:blur(8px); }
.btn-outline:hover { background:#fff; color:var(--primary); }

.stats { position:relative; margin-top:-45px; z-index:20; }
.stats-grid { display:grid; grid-template-columns:repeat(4,1fr); gap:15px; }
.stat-card { background:var(--surface); border:1px solid var(--border); border-radius:20px; padding:22px; text-align:center; box-shadow:var(--shadow); }
.stat-number { color:var(--primary); font-size:30px; font-weight:900; }
.stat-label { color:var(--text-soft); font-size:14px; font-weight:600; }

section.content-section { padding:80px 0; }
.section-heading { text-align:center; margin-bottom:45px; }
.section-label { display:inline-block; color:var(--gold-dark); font-size:14px; font-weight:800; margin-bottom:5px; }
.section-title { font-size:clamp(27px,4vw,42px); color:var(--primary); font-weight:900; line-height:1.35; margin-bottom:12px; }

.about-grid { display:grid; grid-template-columns:1.2fr .8fr; gap:30px; align-items:stretch; }
.card { background:var(--surface); border:1px solid var(--border); border-radius:var(--radius); padding:30px; box-shadow:var(--shadow); }
.card h3 { color:var(--primary); font-size:23px; margin-bottom:14px; font-weight:900; }
.card p { color:var(--text-soft); margin-bottom:14px; }
.quote-card { background:linear-gradient(135deg, var(--primary-dark), var(--primary)); color:#fff; position:relative; overflow:hidden; }
.quote-card h3 { color:var(--gold); }
.quote-card p { color:#fff; }

.pecs-phases { display:grid; grid-template-columns:repeat(auto-fit, minmax(200px, 1fr)); gap:13px; margin-bottom:30px; }
.phase-card { background:var(--surface); border:1px solid var(--border); border-radius:18px; padding:20px; box-shadow:var(--shadow); }
.phase-card h3 { color:var(--primary); font-size:18px; margin-bottom:8px; }
.phase-card p { color:var(--text-soft); font-size:13px; }

/* CONTACT FORM STYLES */
.negin-contact-section { width: min(950px, calc(100% - 30px)); margin: 60px auto; padding: 45px 30px; background: #ffffff; border-radius: 28px; border: 1px solid #d8e1e8; box-shadow: 0 20px 60px rgba(15, 23, 42, .10); direction: rtl; }
.negin-contact-header { text-align: center; margin-bottom: 35px; }
.negin-contact-badge { display: inline-block; padding: 8px 16px; border-radius: 50px; background: #eef5f8; color: #075985; font-weight: 800; font-size: 13px; margin-bottom: 15px; }
.negin-contact-header h2 { margin: 0 0 12px; color: #043b4d; font-size: clamp(24px, 4vw, 34px); font-weight: 900; }
.negin-contact-header p { max-width: 700px; margin: auto; color: #475569; line-height: 2; font-size: 15px; }
.negin-contact-form { width: 100%; }
.negin-form-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 20px; }
.negin-form-group { margin-bottom: 20px; }
.negin-form-group label { display: block; margin-bottom: 8px; color: #172033; font-weight: 800; font-size: 14px; }
.negin-form-group label span { color: #dc2626; }
.negin-form-group input, .negin-form-group select, .negin-form-group textarea { width: 100%; border: 1px solid #d8e1e8; border-radius: 14px; background: #ffffff; color: #172033; padding: 13px 15px; font-family: "Tajawal", "Vazirmatn", Arial, sans-serif; font-size: 14px; outline: none; transition: .25s ease; }
.negin-form-group input, .negin-form-group select { height: 52px; }
.negin-form-group textarea { resize: vertical; min-height: 150px; line-height: 2; }
.negin-form-group input:focus, .negin-form-group select:focus, .negin-form-group textarea:focus { border-color: #0ea5e9; box-shadow: 0 0 0 4px rgba(14, 165, 233, .12); }
.negin-form-group input::placeholder, .negin-form-group textarea::placeholder { color: #94a3b8; }
.negin-consent { display: flex; align-items: flex-start; gap: 10px; padding: 15px; margin: 5px 0 20px; border-radius: 14px; background: #f7fafc; border: 1px solid #e9edf2; color: #475569; font-size: 13px; line-height: 1.9; cursor: pointer; }
.negin-consent input { width: 19px; height: 19px; flex: 0 0 19px; margin-top: 3px; accent-color: #075985; }
.negin-submit { width: 100%; min-height: 56px; border: 1px solid #c99d00; border-radius: 15px; background: #ffc800; color: #111111; font-family: "Tajawal", "Vazirmatn", Arial, sans-serif; font-size: 16px; font-weight: 900; cursor: pointer; transition: .25s ease; }
.negin-submit:hover { background: #e6b400; transform: translateY(-2px); box-shadow: 0 12px 30px rgba(201, 157, 0, .20); }
.negin-submit:active { transform: scale(.98); }
.negin-email-note { text-align: center; margin: 18px 0 0; color: #64748b; font-size: 12px; line-height: 1.8; }
.negin-email-note strong { color: #075985; direction: ltr; display: inline-block; }

.social-links { display: flex; justify-content: center; gap: 15px; margin-top: 20px; flex-wrap: wrap; }
.social-icon { display: inline-flex; align-items: center; justify-content: center; width: 42px; height: 42px; border-radius: 50%; background: rgba(255,255,255,0.1); color: #fff; font-size: 20px; transition: .3s; }
.social-icon:hover { background: var(--gold); color: #111; transform: translateY(-3px); }

@media (max-width: 650px) {
    .negin-contact-section { width: calc(100% - 20px); margin: 35px auto; padding: 30px 17px; border-radius: 22px; }
    .negin-form-grid { grid-template-columns: 1fr; gap: 0; }
    .negin-contact-header h2 { font-size: 23px; }
    .negin-contact-header p { font-size: 13px; }
    .negin-form-group input, .negin-form-group select { height: 50px; }
    .negin-submit { min-height: 54px; font-size: 15px; }
    .stats-grid { grid-template-columns: 1fr; }
    .about-grid { grid-template-columns: 1fr; }
    .brand-logo { height:50px; }
}

body.dark .negin-contact-section { background: #102129; border-color: #29404a; }
body.dark .negin-contact-badge { background: #142b34; color: #52b9a8; }
body.dark .negin-contact-header h2, body.dark .negin-form-group label { color: #f1f5f9; }
body.dark .negin-contact-header p, body.dark .negin-consent, body.dark .negin-email-note { color: #cbd5e1; }
body.dark .negin-form-group input, body.dark .negin-form-group select, body.dark .negin-form-group textarea { background: #102129; color: #f1f5f9; border-color: #29404a; }
body.dark .negin-consent { background: #142b34; border-color: #29404a; }

footer { background:var(--primary-dark); color:#fff; padding:40px 0; text-align:center; font-size:14px; margin-top:50px; }
</style>
</head>

<body>

<a href="#main-content" class="skip-link">پرش به محتوای اصلی</a>

<!-- TOPBAR -->
<div class="topbar">
    <div class="container topbar-inner">
        <div class="topbar-contact">
            <span>📞 ۰۷۸۶۸۳۸۰۰۲</span>
            <span>📧 negineducationcenter@gmail.com</span>
        </div>
        <div>🌐 کابل، پروژه وزیرآباد، سرک ۳۷</div>
    </div>
</div>

<!-- HEADER -->
<header class="main-header">
    <div class="container header-inner">
        <div class="menu-side">
            <button class="icon-btn" id="menuOpenBtn" aria-label="منو">
                <svg viewBox="0 0 24 24"><path d="M4 6h16M4 12h16M4 18h16"></path></svg>
            </button>
        </div>
        
        <!-- DIRECT LOGO -->
        <div class="brand">
            <a href="#" class="brand-logo-wrapper" title="مرکز آموزشی و توانبخشی نگین">
                <img src="https://lh3.googleusercontent.com/d/1xFpErV2qCevAlACuaP2vpKcIwjzsOOZP" alt="لوگوی مرکز آموزشی و توانبخشی نگین" class="brand-logo">
            </a>
        </div>

        <div class="header-actions">
            <button class="icon-btn" id="themeToggleBtn" aria-label="تغییر تم">
                <svg viewBox="0 0 24 24"><circle cx="12" cy="12" r="5"></circle><path d="M12 1v2M12 21v2M4.22 4.22l1.42 1.42M18.36 18.36l1.42 1.42M1 12h2M21 12h2M4.22 19.78l1.42-1.42M18.36 5.64l1.42-1.42"></path></svg>
            </button>
        </div>
    </div>
</header>

<!-- SIDE MENU -->
<div class="menu-overlay" id="menuOverlay"></div>
<aside class="side-menu" id="sideMenu">
    <div class="menu-head">
        <span class="menu-head-title">منوی اصلی</span>
        <button class="menu-close" id="menuCloseBtn">&times;</button>
    </div>
    <ul class="menu-list">
        <li><a href="#about"><span class="menu-icon">🏫</span> درباره مرکز</a></li>
        <li><a href="#services"><span class="menu-icon">🧩</span> خدمات و فعالیت‌ها</a></li>
        <li><a href="#contact-form"><span class="menu-icon">📩</span> فرم ارتباط و ثبت‌نام</a></li>
    </ul>
</aside>

<!-- MAIN CONTENT -->
<main id="main-content">

    <!-- HERO -->
    <section class="hero">
        <div class="hero-slider">
            <div class="hero-slide active"></div>
            <div class="hero-slide"></div>
            <div class="hero-slide"></div>
            <div class="hero-slide"></div>
        </div>
        <div class="container hero-content">
            <div class="hero-text">
                <span class="hero-kicker">آموزش، توان‌بخشی و رشد مهارت‌ها</span>
                <h1 class="hero-title">فرصت‌های برابر برای <span>همه کودکان</span></h1>
                <p class="hero-subtitle">مرکز آموزشی و توان‌بخشی نگین با هدف حمایت، توانمندسازی و فراهم‌سازی زمینه آموزش استاندارد برای کودکان دارای نیازهای ویژه در افغانستان فعالیت می‌کند.</p>
                <div class="hero-buttons">
                    <a href="#contact-form" class="btn btn-gold">ثبت‌نام و درخواست ارتباط</a>
                    <a href="#about" class="btn btn-outline">درباره ما بیشتر بدانید</a>
                </div>
            </div>
        </div>
    </section>

    <!-- STATS -->
    <div class="container stats">
        <div class="stats-grid">
            <div class="stat-card">
                <div class="stat-number">۱۰۰٪</div>
                <div class="stat-label">تعهد به خدمات انسانی</div>
            </div>
            <div class="stat-card">
                <div class="stat-number">۸+</div>
                <div class="stat-label">خدمات تخصصی توان‌بخشی</div>
            </div>
            <div class="stat-card">
                <div class="stat-number">۶</div>
                <div class="stat-label">روز در هفته فعالیت</div>
            </div>
            <div class="stat-card">
                <div class="stat-number">۱</div>
                <div class="stat-label">هدف: رشد و استقلال کودک</div>
            </div>
        </div>
    </div>

    <!-- ABOUT -->
    <section id="about" class="content-section">
        <div class="container">
            <div class="section-heading">
                <span class="section-label">شناخت مرکز</span>
                <h2 class="section-title">درباره مرکز آموزشی و توان‌بخشی نگین</h2>
            </div>
            <div class="about-grid">
                <div class="card">
                    <h3>داستان نگین</h3>
                    <p>نگین از یک باور انسانی و روشن آغاز شده است: «هر کودک توانایی‌هایی دارد که باید دیده، شناخته و پرورش داده شود.»</p>
                    <p>نیاز کودکان دارای معلولیت و نیازهای ویژه تنها به آموزش محدود نمی‌شود. بسیاری از آنان به توان‌بخشی، حمایت خانواده، ابزارهای کمکی و توجه تخصصی نیاز دارند. مرکز نگین با همین هدف شکل گرفته است تا بخشی از این نیازها را پاسخ دهد.</p>
                </div>
                <div class="card quote-card">
                    <h3>دیدگاه ما</h3>
                    <p>ما به جامعه‌ای باور داریم که در آن هیچ کودک دارای معلولیت یا نیاز ویژه‌ای از آموزش، توان‌بخشی، ارتباط و فرصت رشد محروم نباشد.</p>
                    <p><strong>«با اراده می‌توان، با همت می‌سازیم»</strong></p>
                </div>
            </div>
        </div>
    </section>

    <!-- SERVICES -->
    <section id="services" class="content-section">
        <div class="container">
            <div class="section-heading">
                <span class="section-label">ارائه خدمات</span>
                <h2 class="section-title">خدمات و زمینه‌های فعالیت</h2>
            </div>
            <div class="pecs-phases">
                <div class="phase-card">
                    <h3>📚 آموزش ویژه</h3>
                    <p>برنامه‌های آموزشی مناسب با سطح توانایی و شرایط کودک.</p>
                </div>
                <div class="phase-card">
                    <h3>♿ توان‌بخشی</h3>
                    <p>تقویت مهارت‌های جسمی، حرکتی و اجتماعی.</p>
                </div>
                <div class="phase-card">
                    <h3>🗣️ گفتاردرمانی</h3>
                    <p>ارتقای توانایی‌های ارتباطی و کلامی کودکان.</p>
                </div>
                <div class="phase-card">
                    <h3>👐 کاردرمانی</h3>
                    <p>تقویت مهارت‌های روزمره و مشارکت اجتماعی.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- CONTACT & REGISTRATION FORM -->
    <section id="contact-form" class="negin-contact-section">
        <div class="negin-contact-header">
            <span class="negin-contact-badge">📩 ارتباط با نگین</span>
            <h2>با مرکز آموزشی و توانبخشی نگین در تماس باشید</h2>
            <p>برای ثبت درخواست، دریافت اطلاعات، همکاری، داوطلبی، حمایت از کودکان یا پرسش درباره خدمات مرکز، فرم زیر را تکمیل کنید.</p>
        </div>
        <form class="negin-contact-form" action="https://formsubmit.co/negineducationcenter@gmail.com" method="POST">
            <input type="hidden" name="_subject" value="پیام جدید از وبسایت مرکز آموزشی و توانبخشی نگین">
            <input type="hidden" name="_template" value="table">
            <input type="hidden" name="_captcha" value="true">

            <div class="negin-form-grid">
                <div class="negin-form-group">
                    <label for="name"> نام و نام خانوادگی <span>*</span> </label>
                    <input type="text" id="name" name="نام و نام خانوادگی" placeholder="نام و نام خانوادگی خود را وارد کنید" required autocomplete="name">
                </div>
                <div class="negin-form-group">
                    <label for="phone"> شماره تماس <span>*</span> </label>
                    <input type="tel" id="phone" name="شماره تماس" placeholder="مثلاً ۰۷۸۶۸۳۸۰۰۲" required autocomplete="tel">
                </div>
                <div class="negin-form-group">
                    <label for="email"> ایمیل </label>
                    <input type="email" id="email" name="ایمیل فرستنده" placeholder="example@gmail.com" autocomplete="email">
                </div>
                <div class="negin-form-group">
                    <label for="request"> موضوع درخواست <span>*</span> </label>
                    <select id="request" name="موضوع درخواست" required>
                        <option value="">موضوع را انتخاب کنید</option>
                        <option value="ثبت نام کودک"> 🧒 ثبت‌نام کودک </option>
                        <option value="درخواست خدمات توانبخشی"> ♿ درخواست خدمات توانبخشی </option>
                        <option value="آموزش ویژه"> 📚 آموزش ویژه </option>
                        <option value="فیزیوتراپی"> 🏃 فیزیوتراپی </option>
                        <option value="کاردرمانی"> 🤲 کاردرمانی </option>
                        <option value="گفتاردرمانی"> 🗣️ گفتاردرمانی </option>
                        <option value="روانشناسی و مشاوره"> 🧠 روان‌شناسی و مشاوره </option>
                        <option value="کمک مالی"> 💛 کمک مالی </option>
                        <option value="داوطلبی"> 🤝 داوطلبی </option>
                        <option value="همکاری سازمانی"> 🏢 همکاری سازمانی </option>
                        <option value="سایر"> 💬 سایر </option>
                    </select>
                </div>
                <div class="negin-form-group">
                    <label for="child-name"> نام کودک </label>
                    <input type="text" id="child-name" name="نام کودک" placeholder="در صورت نیاز">
                </div>
                <div class="negin-form-group">
                    <label for="child-age"> سن کودک </label>
                    <input type="number" id="child-age" name="سن کودک" min="1" max="30" placeholder="سن کودک">
                </div>
            </div>

            <div class="negin-form-group">
                <label for="disability"> نوع نیاز یا معلولیت </label>
                <select id="disability" name="نوع نیاز یا معلولیت">
                    <option value="">انتخاب کنید</option>
                    <option value="اوتیسم">🧩 اوتیسم</option>
                    <option value="ADHD">⚡ ADHD</option>
                    <option value="معلولیت حرکتی">♿ معلولیت حرکتی</option>
                    <option value="معلولیت بینایی">👁️ معلولیت بینایی</option>
                    <option value="معلولیت شنوایی">👂 معلولیت شنوایی</option>
                    <option value="اختلال گفتار و زبان">🗣️ گفتار و زبان</option>
                    <option value="ناتوانی یادگیری">📖 ناتوانی یادگیری</option>
                    <option value="کم‌توانی ذهنی">🧠 کم‌توانی ذهنی</option>
                    <option value="چندمعلولیتی">🔗 چندمعلولیتی</option>
                    <option value="سایر">سایر</option>
                </select>
            </div>

            <div class="negin-form-group">
                <label for="message"> پیام شما <span>*</span> </label>
                <textarea id="message" name="پیام" rows="7" placeholder="پیام، پرسش یا درخواست خود را اینجا بنویسید..." required></textarea>
            </div>

            <label class="negin-consent">
                <input type="checkbox" name="رضایت" value="با ارسال این فرم، با ارسال اطلاعات برای مرکز موافقم." required>
                <span> با ارسال این فرم، با استفاده از اطلاعات واردشده برای پاسخ‌گویی به درخواست من موافقم. </span>
            </label>

            <button type="submit" class="negin-submit">
                <span>📨</span> ارسال درخواست
            </button>
            <p class="negin-email-note">
                📧 پیام شما مستقیماً به ایمیل مرکز ارسال می‌شود: <strong>negineducationcenter@gmail.com</strong>
            </p>
        </form>
    </section>

</main>

<!-- FOOTER -->
<footer>
    <div class="container">
        <p><strong>مرکز آموزشی و توان‌بخشی نگین</strong> — کلیه حقوق محفوظ است © ۲۰۲۶</p>
        <p>نشانی: کابل، پروژه وزیرآباد، سرک ۳۷ | شماره تماس: ۰۷۸۶۸۳۸۰۰۲</p>
        
        <div class="social-links">
            <a href="#" class="social-icon" aria-label="فیسبوک">🌐</a>
            <a href="#" class="social-icon" aria-label="اینستاگرام">📷</a>
            <a href="#" class="social-icon" aria-label="واتساپ">💬</a>
            <a href="#" class="social-icon" aria-label="تلگرام">✈️</a>
        </div>
    </div>
</footer>

<script>
    // Toggle Side Menu
    const menuOpenBtn = document.getElementById('menuOpenBtn');
    const menuCloseBtn = document.getElementById('menuCloseBtn');
    const sideMenu = document.getElementById('sideMenu');
    const menuOverlay = document.getElementById('menuOverlay');

    function openMenu() {
        sideMenu.classList.add('open');
        menuOverlay.classList.add('show');
    }

    function closeMenu() {
        sideMenu.classList.remove('open');
        menuOverlay.classList.remove('show');
    }

    menuOpenBtn.addEventListener('click', openMenu);
    menuCloseBtn.addEventListener('click', closeMenu);
    menuOverlay.addEventListener('click', closeMenu);

    // Theme Toggle
    const themeToggleBtn = document.getElementById('themeToggleBtn');
    themeToggleBtn.addEventListener('click', () => {
        document.body.classList.toggle('dark');
    });

    // Automatic Hero Slider
    const slides = document.querySelectorAll('.hero-slide');
    let currentSlide = 0;
    setInterval(() => {
        slides[currentSlide].classList.remove('active');
        currentSlide = (currentSlide + 1) % slides.length;
        slides[currentSlide].classList.add('active');
    }, 5000);
</script>

</body>
</html>
