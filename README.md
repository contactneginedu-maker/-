<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>مرکز آموزشی و توانبخشی نگین | هر کودک یک نگین</title>
    <link href="https://cdn.jsdelivr.net/gh/rastikerdar/vazirmatn@v33.003/Vazirmatn-font-face.css" rel="stylesheet" type="text/css" />
    <style>
        :root {
            --primary-color: #0e7490;
            --primary-hover: #155e75;
            --secondary-color: #f59e0b;
            --accent-color: #06b6d4;
            --bg-light: #f8fafc;
            --text-dark: #1e293b;
            --text-muted: #64748b;
            --white: #ffffff;
            --card-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.05), 0 4px 6px -2px rgba(0, 0, 0, 0.025);
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Vazirmatn', sans-serif;
            background-color: var(--bg-light);
            color: var(--text-dark);
            line-height: 1.8;
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        header {
            background: linear-gradient(135deg, #0f172a 0%, var(--primary-color) 100%);
            color: var(--white);
            padding: 60px 20px;
            text-align: center;
            border-bottom: 5px solid var(--secondary-color);
        }

        .sub-title {
            font-size: 1.1rem;
            font-weight: 300;
            letter-spacing: 1px;
            color: #cbd5e1;
            margin-bottom: 8px;
        }

        .main-title {
            font-size: 2.8rem;
            font-weight: 900;
            margin-bottom: 15px;
            color: var(--white);
        }

        .slogan {
            display: inline-block;
            background-color: var(--secondary-color);
            color: #000;
            padding: 6px 24px;
            border-radius: 50px;
            font-weight: 700;
            font-size: 1.2rem;
            margin-top: 10px;
        }

        /* Sections General */
        section {
            padding: 60px 0;
            border-bottom: 1px solid #e2e8f0;
        }

        .section-title {
            text-align: center;
            font-size: 2rem;
            color: var(--primary-color);
            margin-bottom: 40px;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 70px;
            height: 4px;
            background-color: var(--secondary-color);
            margin: 10px auto 0;
            border-radius: 2px;
        }

        .text-content {
            font-size: 1.1rem;
            text-align: justify;
            color: var(--text-dark);
            background: var(--white);
            padding: 30px;
            border-radius: 12px;
            box-shadow: var(--card-shadow);
            margin-bottom: 25px;
        }

        .highlight-quote {
            background-color: #ecfeff;
            border-right: 4px solid var(--accent-color);
            padding: 20px;
            margin: 20px 0;
            font-style: italic;
            border-radius: 0 8px 8px 0;
        }

        /* Quotes / Messages */
        .quote-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
        }

        .quote-card {
            background: var(--white);
            padding: 25px;
            border-radius: 12px;
            box-shadow: var(--card-shadow);
            border-top: 4px solid var(--primary-color);
        }

        .quote-author {
            margin-top: 15px;
            font-weight: 700;
            color: var(--primary-color);
            text-align: left;
        }

        /* Special Section: Ajmir Khan Mirzad */
        .special-feature {
            background: linear-gradient(to bottom, #ffffff, #f0f9ff);
            border: 2px solid #bae6fd;
            border-radius: 16px;
            padding: 40px;
            margin: 40px 0;
            box-shadow: var(--card-shadow);
        }

        .special-feature h3 {
            color: var(--primary-color);
            margin-top: 25px;
            margin-bottom: 10px;
        }

        .badge {
            display: inline-block;
            background-color: #e0f2fe;
            color: var(--primary-color);
            padding: 4px 12px;
            border-radius: 6px;
            font-size: 0.9rem;
            font-weight: 600;
            margin-bottom: 15px;
        }

        /* Cards Grid (Vision/Mission/Values) */
        .grid-3 {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
        }

        .card {
            background: var(--white);
            padding: 25px;
            border-radius: 12px;
            box-shadow: var(--card-shadow);
            transition: transform 0.2s;
        }

        .card:hover {
            transform: translateY(-5px);
        }

        .card h3 {
            color: var(--primary-color);
            margin-bottom: 15px;
        }

        /* Team Section */
        .team-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .team-member {
            background: var(--white);
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            box-shadow: var(--card-shadow);
        }

        .team-member h4 {
            color: var(--primary-color);
            font-size: 1.2rem;
        }

        .team-member p.role {
            color: var(--text-muted);
            font-size: 0.95rem;
            margin-bottom: 10px;
            font-weight: 600;
        }

        /* Contact Info */
        .contact-box {
            background: var(--white);
            padding: 30px;
            border-radius: 12px;
            box-shadow: var(--card-shadow);
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
        }

        .contact-item {
            margin-bottom: 15px;
        }

        .contact-item strong {
            display: block;
            color: var(--primary-color);
            margin-bottom: 5px;
        }

        .btn-map {
            display: inline-block;
            background-color: var(--primary-color);
            color: var(--white);
            padding: 8px 16px;
            border-radius: 6px;
            text-decoration: none;
            margin-top: 5px;
            font-size: 0.9rem;
            transition: background-color 0.2s;
        }

        .btn-map:hover {
            background-color: var(--primary-hover);
        }

        /* Responsive */
        @media (max-width: 768px) {
            .main-title { font-size: 2rem; }
            .sub-title { font-size: 0.95rem; }
            .slogan { font-size: 1rem; }
            .special-feature { padding: 20px; }
        }
    </style>
</head>
<body>

<!-- هدر وبسایت (Header) -->
<header>
    <div class="container">
        <div class="sub-title">مؤسسه‌ی خدماتی و حرفوی زنان بی‌بضاعت</div>
        <h1 class="main-title">مرکز آموزشی و توانبخشی نگین</h1>
        <div class="slogan">شعار: «هر کودک یک نگین»</div>
    </div>
</header>

<div class="container">

    <!-- درباره ما & معرفی کوتاه -->
    <section id="about">
        <h2 class="section-title">درباره ما</h2>
        <div class="text-content">
            <h3>سلام، ما نگین هستیم.</h3>
            <p>مرکز آموزشی و توانبخشی نگین، ثمره‌ی سال‌ها عشق و تلاش اسدالله و ساحل حیدری است که با همراهی نیکوکارانه‌ی اجمیر خان میرزاد، امروز به خانه‌ای امن برای کودکان دارای معلولیت در کابل تبدیل شده است. اینجا، ما به هر کودکی می‌آموزیم که می‌تواند، همان‌طور که دیگران می‌توانند.</p>
            <p>ما باور داریم که هیچ کودکی نباید به خاطر تفاوت‌هایش از آموزش و فرصت‌های زندگی محروم بماند. مرکز نگین، پاسخی است به سال‌ها بی‌پاسخی و پناهی است برای کودکانی که جامعه آن‌ها را فراموش کرده بود.</p>
        </div>
    </section>

    <!-- داستان نگین -->
    <section id="story">
        <h2 class="section-title">داستان نگین؛ رویایی که به واقعیت پیوست</h2>
        <div class="text-content">
            <p>مرکز آموزشی و توانبخشی نگین، حاصل سال‌ها آرزوی اسدالله حیدری و ساحل حیدری است. آنان که سال‌ها در میان کودکان دارای معلولیت زیستند و با چشم‌های خود، محرومیت‌های بی‌شمار این کودکان را دیدند، تصمیم گرفتند که تغییری اساسی ایجاد کنند.</p>
            <p>سال‌ها تلاش، پیگیری و دل‌سپردن به ناامیدی‌های مکرر، سرانجام با همراهی ارزشمند اجمیر خان میرزاد، پسر جوان و نیکوکاری که دل در گروِ خدمت به همنوع داشت، به ثمر نشست. اجمیر خان با دانش، انرژی و سرمایه‌ی وجودی خود، پل شد میان یک رؤیای دیرینه و یک واقعیت ملموس.</p>
            <p>امروز، مرکز نگین به عنوان یکی از معدود مراکز تخصصی آموزشی و توانبخشی کودکان دارای معلولیت در کابل، پناهگاهی امن برای کودکانی است که جامعه آن‌ها را فراموش کرده بود.</p>
        </div>
    </section>

    <!-- پیام بنیان‌گذاران -->
    <section id="messages">
        <h2 class="section-title">پیام بنیان‌گذاران</h2>
        <div class="quote-grid">
            <div class="quote-card">
                <p>«سال‌ها پیش، وقتی به چشم‌های پرامید کودکان دارای معلولیت نگاه می‌کردیم، به خود قول دادیم که روزی خانه‌ای برای آن‌ها بسازیم. خانه‌ای که در آن، کسی به خاطر تفاوت‌هایش طرد نشود؛ خانه‌ای که در آن، هر کودکی بتواند پرواز کند. امروز، با کمک شما، آن قول را عملی می‌کنیم.»</p>
                <div class="quote-author">— اسدالله حیدری و ساحل حیدری، بنیان‌گذاران</div>
            </div>
            <div class="quote-card">
                <p>«این مرکز، فقط یک ساختمان نیست؛ پاسخی است به سال‌ها بی‌پاسخی. من به این راه افتخار می‌کنم و از همه دعوت می‌کنم که در این مسیر انسانی همراه ما باشند.»</p>
                <div class="quote-author">— اجمیر خان میرزاد<br><small>«با اراده می‌توان، با همت می‌سازیم»</small></div>
            </div>
        </div>
    </section>

    <!-- نقش اجمیر خان میرزاد -->
    <section id="ajmir-khan">
        <div class="special-feature">
            <h2 style="color: var(--primary-color); text-align: center; margin-bottom: 10px;">نقش اجمیر خان میرزاد؛ جوانی که رؤیا را به واقعیت پیوند زد</h2>
            <div style="text-align: center;">
                <span class="badge">مشاور ارشد و حامی کلیدی مرکز آموزشی و توانبخشی نگین</span>
                <p style="font-weight: bold; color: var(--secondary-color); margin-bottom: 20px;">«با اراده می‌توان، با همت می‌سازیم»</p>
            </div>
            
            <p>در مسیر طولانی و پرپیچ‌وخم تحقق مرکز نگین، نقطه‌ی عطفی وجود دارد که نمی‌توان از آن گذشت؛ نقطه‌ای که در آن، یک رؤیای دیرینه به یک تعهد عملی تبدیل شد. آن نقطه، حضور اجمیر خان میرزاد، پسر جوانی است که با دلی سرشار از مهر انسانی و همتی والا، پا به میدان گذاشت و مسیر تاریخ این مرکز را برای همیشه تغییر داد.</p>

            <h3>کسی که آمد تا بماند</h3>
            <p>اجمیر خان میرزاد، جوانی است که در دوران پرالتهاب زندگی‌اش، دغدغه‌ای بزرگ در دل داشت: خدمت به همنوع. او که از نزدیک شاهد درد و رنج خانواده‌های دارای کودکان معلول بود، نمی‌توانست بی‌تفاوت بماند. آنچه اجمیر خان را از دیگران متمایز می‌کند، نه تنها سخاوت مالی او، بلکه حضورِ قلبی و عاطفی‌اش در کنار این مرکز است.</p>
            <p>او وقتی با آرزوی اسدالله و ساحل حیدری آشنا شد، نه به عنوان یک ناظر، بلکه به عنوان یک شریکِ راه، آستین همت را بالا زد. اجمیر خان به خوبی می‌دانست که ساختن یک مرکز آموزشی و توانبخشی فقط به پول نیاز ندارد؛ به عشق، زمان، انرژی و تعهدِ بی‌دریغ نیز نیاز است. و او همه‌ی این‌ها را با خود آورد.</p>

            <h3>پلی از جنس امید</h3>
            <p>اجمیر خان با دانش، بینش و سرمایه‌ی وجودی خود، پل شد میان یک رویای دست‌نیافتنی و یک واقعیت ملموس. او با برنامه‌ریزی دقیق، پیگیری‌های مستمر و حمایت‌های بی‌وقفه‌ی خود، زمینه‌ی راه‌اندازی این مرکز را فراهم کرد. او نه فقط تأمین کننده‌ی منابع مالی، که مشاوری امین، همراهی دلسوز و حامی‌ای قدرتمند برای تیم بنیان‌گذار بود.</p>
            <p>در روزهایی که ناامیدی بر دل‌ها سنگینی می‌کرد، اجمیر خان با روحیه‌ی جوانی و ایمان راسخ خود، امید را به تیم بازگرداند. او بارها و بارها نشان داد که برایش موفقیت این پروژه، فقط یک تعهد مالی نیست؛ یک آرزوی قلبی است که به دوش کشیده است. هر وقت صحبت از کودکان دارای معلولیت می‌شد، چشمانش از عشق و دلسوزی می‌درخشید و همین عشق، انگیزه‌ای شد برای همه‌ی کسانی که در این راه قدم برداشتند.</p>

            <h3>افتخاری برای نسل جوان</h3>
            <p>اجمیر خان میرزاد، نماد نسل جوانِ بیدار، مسئول و انسان‌دوست افغانستان است. نسلی که با وجود تمام مشکلات و ناامیدی‌های پیرامون، هنوز هم به ساختن و خدمت به همنوع باور دارد. او ثابت کرد که برای تغییر، نیازی به منتظر ماندن نیست؛ با اراده و همت می‌توان آغاز کرد.</p>
            
            <div class="highlight-quote">
                <p>او در یکی از پیام‌هایش گفت:</p>
                <p><strong>«این مرکز، فقط یک ساختمان نیست؛ پاسخی است به سال‌ها بی‌پاسخی. من به این راه افتخار می‌کنم و از همه دعوت می‌کنم که در این مسیر انسانی همراه ما باشند.»</strong></p>
                <p style="margin-top: 5px;">— اجمیر خان میرزاد («با اراده می‌توان، با همت می‌سازیم»)</p>
            </div>

            <p>این کلمات، نه یک شعار، که باورِ عمیقِ او را نشان می‌دهد. اجمیر خان با عمل خود، به همه‌ی جوانان این سرزمین پیام داد که هر کسی، در هر جایگاهی، می‌تواند بخشی از یک تغییر بزرگ باشد.</p>

            <h3>تأثیر حضور او در مرکز نگین</h3>
            <p>حضور اجمیر خان در مرکز نگین، فراتر از یک حمایت مالی، روحیه‌ی تازه‌ای به تیم بخشیده و اعتمادبه‌نفس خانواده‌ها را افزایش داده است. او نه تنها در مراحل راه‌اندازی، بلکه در ادامه‌ی مسیر نیز به‌عنوان مشاور ارشد و حامی کلیدی در کنار مرکز باقی خواهد ماند. برنامه‌های او برای آینده شامل گسترش خدمات، جذب خیرین بیشتر و ایجاد شبکه‌ای از حمایت‌های پایدار برای کودکان دارای معلولیت است.</p>
            <p>اجمیر خان باور دارد که هر کودکی، فارغ از هر محدودیتی، شایسته‌ی یک زندگیِ باکرامت است و به همین دلیل، هیچ‌گاه از تلاش برای بهبود شرایط این کودکان دست نخواهد کشید.</p>

            <h3>سپاس از همراهی بی‌نظیر او</h3>
            <p>مرکز آموزشی و توانبخشی نگین، امروز به برکت وجود انسان‌هایی مانند اجمیر خان میرزاد، بر پا ایستاده است. اسدالله و ساحل حیدری، بارها از حمایت‌های بی‌دریغ او سخن گفته‌اند و او را نور امیدی در تاریکیِ سال‌های دشوار خوانده‌اند.</p>
            <p>ما در مرکز نگین، به وجود چنین همراهانی افتخار می‌کنیم و از صمیم قلب، سپاسگزار حضور اجمیر خان میرزاد در کنار خود هستیم. او نشان داد که جوانان این سرزمین، اگر اراده کنند، می‌توانند تاریخ‌ساز شوند.</p>
            <p style="font-weight: bold; text-align: center; margin-top: 15px; color: var(--primary-color);">اجمیر خان میرزاد؛ مردی که با عشقش، نگین را درخشان‌تر کرد. ✨</p>
        </div>
    </section>

    <!-- چشم‌انداز، مأموریت و ارزش‌ها -->
    <section id="vision-mission-values">
        <div class="grid-3">
            <div class="card">
                <h3>چشم‌انداز</h3>
                <p>جامعه‌ای فراگیر که در آن هر کودک دارای معلولیت، فارغ از نوع و شدت آسیب، از حق آموزش باکیفیت و خدمات توانبخشی بهره‌مند شود و بتواند شکوفاترین نسخه خود را در فضایی امن و پویا تجربه کند.</p>
            </div>
            <div class="card">
                <h3>مأموریت</h3>
                <p>ارائه خدمات آموزشی، توانبخشی و حمایتی تخصصی و یکپارچه به کودکان دارای معلولیت، با تکیه بر رویکرد تیمی میان‌رشته‌ای و مشارکت فعال خانواده‌ها، به منظور ارتقای کیفیت زندگی، استقلال و مشارکت اجتماعی این کودکان.</p>
            </div>
            <div class="card">
                <h3>ارزش‌های ما</h3>
                <p><strong>عشق بی‌قیدوشرط:</strong> هر کودکی، مهم نیست با چه توانایی‌هایی، در اینجا پذیرفته و دوست داشته می‌شود. ما به جای نگاه به محدودیت‌ها، به توانایی‌های کودکان نگاه می‌کنیم.</p>
                <p><strong>باور به توانمندی:</strong> ما به هر کودکی می‌آموزیم که می‌تواند. باور به توانمندی‌های کودکان، اساس تمام برنامه‌های ماست.</p>
                <p><strong>همبستگی و مشارکت:</strong> باور داریم که تغییر واقعی، با همکاری خانواده‌ها، جامعه و خیرین امکان‌پذیر است. هیچ‌کس به تنهایی نمی‌تواند، اما همه با هم می‌توانیم.</p>
            </div>
        </div>
    </section>

    <!-- سه محور اصلی فعالیت -->
    <section id="services">
        <h2 class="section-title">سه محور اصلی فعالیت</h2>
        <div class="grid-3">
            <div class="card">
                <h3>آموزش تخصصی</h3>
                <p>برنامه‌های آموزشی فردی‌سازی‌شده با نسبت مربی به دانش‌آموز پایین، تا هر کودک بتواند بهترین نسخه‌ی خود را شکوفا کند.</p>
            </div>
            <div class="card">
                <h3>توانبخشی حرفه‌ای</h3>
                <p>ارائه خدمات فیزیوتراپی، کاردرمانی، گفتاردرمانی و روان‌درمانی برای ارتقای توانایی‌های جسمی، گفتاری و روانی کودکان.</p>
            </div>
            <div class="card">
                <h3>حمایت از خانواده</h3>
                <p>مشاوره، کارگاه‌های آموزشی و حمایت عاطفی از والدین، زیرا می‌دانیم که خانواده، اولین و مهم‌ترین مدرسه‌ی هر کودک است.</p>
            </div>
        </div>
    </section>

    <!-- تیم ما -->
    <section id="team">
        <h2 class="section-title">تیم ما</h2>
        <div class="team-grid">
            <div class="team-member">
                <h4>اسدالله حیدری</h4>
                <p class="role">بنیان‌گذار و مدیر اجرایی</p>
                <p>سال‌ها در حوزه حمایت از کودکان دارای معلولیت فعالیت داشته و با عشق و تعهدی بی‌نظیر، هدایت این مرکز را بر عهده دارد.</p>
            </div>
            <div class="team-member">
                <h4>ساحل حیدری</h4>
                <p class="role">بنیان‌گذار و مدیر آموزشی</p>
                <p>با سال‌ها تجربه در آموزش کودکان دارای نیازهای ویژه، برنامه‌های آموزشی مرکز را طراحی و نظارت می‌کند.</p>
            </div>
            <div class="team-member">
                <h4>اجمیر خان میرزاد</h4>
                <p class="role">مشاور ارشد و حامی کلیدی</p>
                <p>«با اراده می‌توان، با همت می‌سازیم»<br>جوانی انسان‌دوست و خیر که با حمایت‌های بی‌دریغ خود، تحقق این رویا را ممکن ساخت.</p>
            </div>
            <div class="team-member">
                <h4>تیم تخصصی</h4>
                <p class="role">قلب تپنده‌ی نگین</p>
                <p>متشکل از مربیان آموزش ویژه، فیزیوتراپیست‌ها، کاردرمان‌گران، گفتاردرمان‌گران، روان‌شناسان و مددکاران اجتماعی.</p>
            </div>
        </div>
    </section>

    <!-- چرا به نگین نیاز داریم؟ -->
    <section id="why-negin">
        <h2 class="section-title">چرا به نگین نیاز داریم؟</h2>
        <div class="text-content">
            <p>در کشوری که سال‌ها درگیر ناامنی و فقر بوده، کودکان دارای معلولیت، قربانیان خاموش‌ترین و بی‌عدالت‌ترین صحنه‌ها هستند. آنان نه تنها از موهبت‌های اولیه‌ی زندگی مانند آموزش و درمان محرومند، بلکه اغلب پشت درهای بسته‌ی مدارس و درمانگاه‌ها رها می‌شوند.</p>
            <p>مدرسه‌ای که رمپ ندارد، کلاسی که معلم آموزش‌دیده ندارد، درمانگاهی که تجهیزات فیزیوتراپی ندارد—این‌ها واقعیت‌های تلخی هستند که هر روز، زندگی صدها کودک را تحت تأثیر قرار می‌دهند. مرکز نگین آمده است تا بخشی از این خلأ را پر کند.</p>
        </div>
    </section>

    <!-- دعوت به همکاری -->
    <section id="get-involved">
        <h2 class="section-title">دعوت به همکاری</h2>
        <div class="text-content" style="text-align: center;">
            <h3 style="margin-bottom: 15px; color: var(--primary-color);">ما به شما نیاز داریم.</h3>
            <p style="margin-bottom: 20px;">مرکز نگین با عشق ساخته شده، اما برای ادامه‌ی مسیر و کمک به کودکان بیشتر، به حمایت شما نیاز دارد. هر کمکی، هرچند کوچک، برای کودکی که همه‌چیزش را از دست داده، می‌تواند همه‌چیز باشد.</p>
            <p style="text-align: right;"><strong>شما می‌توانید از سه راه به ما کمک کنید:</strong></p>
            <ul style="text-align: right; margin-right: 20px; margin-top: 10px; line-height: 2;">
                <li><strong>کمک مالی:</strong> حتی یک مبلغ کوچک می‌تواند یک جلسه‌ی گفتاردرمانی یا فیزیوتراپی را برای کودکی که به آن نیاز دارد، فراهم کند.</li>
                <li><strong>داوطلبی:</strong> اگر زمان، تخصص یا انرژی برای کمک دارید، به تیم ما بپیوندید.</li>
                <li><strong>همکاری سازمانی:</strong> اگر نهاد، سازمان یا شرکتی هستید که می‌خواهد با ما همکاری کند، با ما تماس بگیرید.</li>
            </ul>
        </div>
    </section>

    <!-- نظرات خانواده‌ها -->
    <section id="testimonials">
        <h2 class="section-title">نظرات خانواده‌ها</h2>
        <div class="quote-grid">
            <div class="quote-card">
                <p>«پسرم قبل از آمدن به نگین، هیچ‌کس به فکر آموزشش نبود. امروز، اولین کلماتش را به زبان آورده و من هر روز برایش می‌خندم. نگین، هدیه‌ای از آسمان بود.»</p>
                <div class="quote-author">— مادر یکی از دانش‌آموزان</div>
            </div>
            <div class="quote-card">
                <p>«وقتی دیدم بچّه‌ام با ویلچر وارد کلاس شد و با لبخند از من خداحافظی کرد، فهمیدم که نگین همان جایی است که سال‌ها دنبالش می‌گشتم.»</p>
                <div class="quote-author">— پدر یکی از دانش‌آموزان</div>
            </div>
        </div>
    </section>

    <!-- اطلاعات تماس -->
    <section id="contact" style="border-bottom: none;">
        <h2 class="section-title">اطلاعات تماس</h2>
        <div class="contact-box">
            <div class="contact-item">
                <strong>بنیان‌گذاران:</strong>
                اسدالله حیدری و ساحل حیدری
            </div>
            <div class="contact-item">
                <strong>مشاور و حامی کلیدی:</strong>
                اجمیر خان میرزاد
            </div>
            <div class="contact-item">
                <strong>شعار اجمیر خان میرزاد:</strong>
                «با اراده می‌توان، با همت می‌سازیم»
            </div>
            <div class="contact-item">
                <strong>آدرس مرکز:</strong>
                سرک ۳۷، پروژه وزیر آباد، کابل، افغانستان
                <br>
                <a href="https://maps.app.goo.gl/UTwdrbUfqR6ewS9D9" target="_blank" class="btn-map">مشاهده در نقشه گوگل 📍</a>
            </div>
            <div class="contact-item">
                <strong>شماره تماس:</strong>
                <span dir="ltr">۰۷۸۶۸۳۸۰۰۲</span>
            </div>
            <div class="contact-item">
                <strong>ایمیل:</strong>
                <span dir="ltr">negineducationcenter@gmail.com</span>
            </div>
            <div class="contact-item" style="grid-column: 1 / -1;">
                <strong>ساعات کاری:</strong>
                شنبه تا چهارشنبه: ۸ صبح تا ۴ بعدازظهر | پنجشنبه: ۸ صبح تا ۱۲ ظهر
            </div>
        </div>
    </section>

</div>

</body>
</html>
