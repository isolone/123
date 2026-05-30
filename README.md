<!doctype html>
<html lang="ru">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Виталий & Дарья — свадебное приглашение</title>
  <meta name="description" content="Свадебное приглашение Виталия и Дарьи — 11.09.2026, Самара" />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;1,300;1,400&family=Jost:wght@300;400;500&display=swap" rel="stylesheet">
  <style>
    :root{
      --black:#050505;
      --wine:#65091b;
      --olive:#4f4b38;
      --taupe:#a18c77;
      --cream:#e7d8ad;
      --paper:#f6f0e1;
      --white:#fffaf0;
      --text:#211d18;
      --muted:#746a5e;
      --line:rgba(33,29,24,.16);
      --shadow:0 24px 70px rgba(5,5,5,.16);
      --radius:28px;
    }

    *{box-sizing:border-box;margin:0;padding:0}
    html{scroll-behavior:smooth}
    body{
      font-family:"Jost",system-ui,-apple-system,BlinkMacSystemFont,"Segoe UI",sans-serif;
      color:var(--text);
      background:
        radial-gradient(circle at 8% 12%, rgba(101,9,27,.16), transparent 30%),
        radial-gradient(circle at 92% 5%, rgba(79,75,56,.18), transparent 34%),
        linear-gradient(135deg,#160d0c 0%,#2a1114 35%,#2d2a21 100%);
      min-height:100vh;
      overflow-x:hidden;
    }

    body::before{
      content:"";
      position:fixed;
      inset:0;
      pointer-events:none;
      background-image:
        linear-gradient(rgba(255,255,255,.03) 1px, transparent 1px),
        linear-gradient(90deg, rgba(255,255,255,.03) 1px, transparent 1px);
      background-size:42px 42px;
      mask-image:linear-gradient(to bottom, rgba(0,0,0,.8), rgba(0,0,0,.12));
      z-index:0;
    }

    a{color:inherit}
    button,input,select,textarea{font:inherit}
    .page{position:relative;z-index:1}
    .container{width:min(1120px, calc(100% - 32px)); margin:0 auto}
    .serif{font-family:"Cormorant Garamond",serif}
    .script{
      font-family:"Cormorant Garamond",serif;
      font-style:italic;
      font-weight:300;
      letter-spacing:.01em;
    }

    .topbar{
      position:fixed;
      left:50%;
      transform:translateX(-50%);
      bottom:18px;
      z-index:50;
      width:min(760px, calc(100% - 28px));
      display:flex;
      justify-content:center;
      gap:4px;
      padding:7px;
      border:1px solid rgba(231,216,173,.22);
      background:rgba(5,5,5,.70);
      backdrop-filter:blur(18px);
      border-radius:999px;
      box-shadow:0 16px 44px rgba(0,0,0,.35);
    }
    .topbar a{
      text-decoration:none;
      color:#f6f0e1;
      font-size:12px;
      letter-spacing:.08em;
      text-transform:uppercase;
      padding:10px 12px;
      border-radius:999px;
      opacity:.82;
      transition:.25s ease;
      white-space:nowrap;
    }
    .topbar a:hover{
      opacity:1;
      background:rgba(231,216,173,.14);
    }

    .hero{
      min-height:100svh;
      display:grid;
      align-items:center;
      padding:70px 0 110px;
      color:var(--white);
      position:relative;
      overflow:hidden;
    }
    .hero::before{
      content:"";
      position:absolute;
      inset:0;
      background:
        linear-gradient(90deg, rgba(5,5,5,.94), rgba(5,5,5,.58) 46%, rgba(5,5,5,.18)),
        radial-gradient(circle at 76% 35%, rgba(101,9,27,.50), transparent 32%),
        radial-gradient(circle at 84% 85%, rgba(231,216,173,.19), transparent 26%);
      z-index:0;
    }
    .hero-inner{
      position:relative;
      z-index:2;
      display:grid;
      grid-template-columns:minmax(0, 1.05fr) minmax(320px,.78fr);
      align-items:center;
      gap:56px;
    }
    .eyebrow{
      display:inline-flex;
      align-items:center;
      gap:12px;
      margin-bottom:22px;
      font-size:12px;
      letter-spacing:.28em;
      text-transform:uppercase;
      color:rgba(246,240,225,.78);
    }
    .eyebrow::before,.eyebrow::after{
      content:"";
      width:34px;
      height:1px;
      background:rgba(231,216,173,.48);
    }
    h1{
      font-size:clamp(68px, 13vw, 160px);
      line-height:.82;
      font-family:"Cormorant Garamond",serif;
      font-weight:300;
      letter-spacing:-.045em;
      text-wrap:balance;
    }
    .amp{
      display:block;
      color:var(--cream);
      font-style:italic;
      font-size:.58em;
      padding:0 0 .03em .12em;
      opacity:.92;
    }
    .hero-text{
      max-width:620px;
      margin-top:28px;
      color:rgba(246,240,225,.78);
      font-size:18px;
      line-height:1.8;
    }
    .hero-actions{
      display:flex;
      gap:14px;
      flex-wrap:wrap;
      margin-top:34px;
    }
    .btn{
      display:inline-flex;
      align-items:center;
      justify-content:center;
      min-height:48px;
      border-radius:999px;
      padding:13px 22px;
      text-decoration:none;
      border:1px solid rgba(231,216,173,.34);
      background:rgba(231,216,173,.11);
      color:var(--white);
      letter-spacing:.12em;
      text-transform:uppercase;
      font-size:12px;
      transition:.25s ease;
      cursor:pointer;
    }
    .btn:hover{transform:translateY(-2px); background:rgba(231,216,173,.20)}
    .btn.primary{background:var(--wine); border-color:rgba(231,216,173,.25)}
    .btn.dark{background:var(--black); color:var(--white)}
    .btn.light{background:var(--paper); color:var(--black); border-color:rgba(5,5,5,.12)}

    .hero-card{
      background:rgba(246,240,225,.94);
      color:var(--text);
      border-radius:36px;
      padding:22px;
      box-shadow:var(--shadow);
      border:1px solid rgba(231,216,173,.35);
      transform:rotate(1.5deg);
    }
    .palette-card{
      min-height:550px;
      border-radius:28px;
      background:
        linear-gradient(rgba(5,5,5,.16), rgba(5,5,5,.58)),
        radial-gradient(circle at 50% 0%, #f8f2e8 0 7%, transparent 8%),
        radial-gradient(circle at 82% 24%, #65091b 0 5%, transparent 6%),
        radial-gradient(circle at 72% 36%, #0b0a09 0 5%, transparent 6%),
        radial-gradient(circle at 70% 50%, #65091b 0 4%, transparent 5%),
        linear-gradient(140deg,#201d16,#4f4b38 38%,#65091b 66%,#080706);
      position:relative;
      overflow:hidden;
      display:grid;
      align-content:end;
      padding:26px;
    }
    .palette-card::before{
      content:"";
      position:absolute;
      width:360px;height:360px;
      right:-90px;top:-46px;
      border-radius:50%;
      background:
        radial-gradient(circle at 45% 45%, #fffaf0 0 28%, transparent 29%),
        radial-gradient(circle at 62% 30%, #0b0a09 0 10%, transparent 11%),
        radial-gradient(circle at 38% 68%, #65091b 0 11%, transparent 12%);
      opacity:.9;
      filter:blur(.2px);
    }
    .palette-card::after{
      content:"";
      position:absolute;
      inset:0;
      background:
        radial-gradient(circle at 20% 72%, rgba(231,216,173,.55), transparent 15%),
        radial-gradient(circle at 28% 70%, rgba(255,255,255,.58), transparent 12%),
        linear-gradient(to top, rgba(5,5,5,.44), transparent 48%);
      pointer-events:none;
    }
    .date-badge{
      position:relative;
      z-index:2;
      display:grid;
      grid-template-columns:1fr auto 1fr;
      align-items:center;
      gap:18px;
      color:var(--white);
    }
    .date-badge span{
      height:1px;
      background:rgba(231,216,173,.45);
    }
    .date-badge strong{
      font-family:"Cormorant Garamond",serif;
      font-weight:300;
      font-size:32px;
      letter-spacing:.04em;
    }
    .palette{
      position:relative;
      z-index:3;
      display:flex;
      justify-content:center;
      gap:10px;
      margin-top:20px;
    }
    .swatch{
      width:48px;
      height:48px;
      border-radius:999px;
      border:2px solid rgba(255,250,240,.8);
      box-shadow:0 12px 24px rgba(0,0,0,.22);
    }

    .petals{position:absolute;inset:0;pointer-events:none;z-index:1}
    .petal{
      position:absolute;
      width:8px;height:13px;
      border-radius:60% 40% 60% 0;
      background:var(--wine);
      opacity:.26;
      animation:fall linear infinite;
    }
    @keyframes fall{
      0%{transform:translateY(-10vh) rotate(0deg); opacity:0}
      10%{opacity:.26}
      100%{transform:translateY(112vh) rotate(420deg); opacity:0}
    }

    section{padding:96px 0}
    .section-light{
      background:var(--paper);
    }
    .section-dark{
      background:
        radial-gradient(circle at 10% 20%, rgba(101,9,27,.25), transparent 30%),
        linear-gradient(135deg, #070706, #1e1b15 55%, #321017);
      color:var(--white);
    }
    .section-head{
      text-align:center;
      max-width:720px;
      margin:0 auto 44px;
    }
    .kicker{
      font-size:12px;
      letter-spacing:.26em;
      text-transform:uppercase;
      color:var(--wine);
      margin-bottom:16px;
    }
    .section-dark .kicker{color:var(--cream)}
    h2{
      font-family:"Cormorant Garamond",serif;
      font-weight:300;
      font-style:italic;
      font-size:clamp(42px, 7vw, 82px);
      line-height:1;
      margin-bottom:18px;
    }
    .lead{
      color:var(--muted);
      font-size:18px;
      line-height:1.85;
    }
    .section-dark .lead{color:rgba(246,240,225,.74)}

    .invite-card{
      border:1px solid var(--line);
      border-radius:var(--radius);
      background:rgba(255,250,240,.48);
      padding:clamp(28px, 5vw, 64px);
      text-align:center;
      box-shadow:0 18px 60px rgba(79,75,56,.10);
      position:relative;
      overflow:hidden;
    }
    .invite-card::before,.invite-card::after{
      content:"";
      position:absolute;
      border-radius:50%;
      border:1px solid rgba(101,9,27,.14);
      width:280px;height:280px;
    }
    .invite-card::before{left:-135px;top:-135px}
    .invite-card::after{right:-135px;bottom:-135px}
    .invite-card p{
      max-width:760px;
      margin:0 auto;
      font-size:20px;
      line-height:1.95;
      position:relative;
      z-index:1;
    }

    .countdown{
      display:grid;
      grid-template-columns:repeat(4,1fr);
      gap:16px;
      margin-top:38px;
    }
    .cd{
      border-radius:24px;
      padding:24px 14px;
      background:#fffaf0;
      border:1px solid var(--line);
      text-align:center;
    }
    .cd-num{
      font-family:"Cormorant Garamond",serif;
      font-size:clamp(38px,5vw,64px);
      line-height:1;
      font-weight:300;
      color:var(--wine);
    }
    .cd-label{
      margin-top:8px;
      text-transform:uppercase;
      letter-spacing:.18em;
      font-size:11px;
      color:var(--muted);
    }

    .details-grid{
      display:grid;
      grid-template-columns:repeat(3,1fr);
      gap:18px;
    }
    .detail{
      background:rgba(255,250,240,.08);
      border:1px solid rgba(231,216,173,.16);
      border-radius:var(--radius);
      padding:28px;
      min-height:220px;
      display:flex;
      flex-direction:column;
      justify-content:space-between;
      box-shadow:0 20px 50px rgba(0,0,0,.12);
    }
    .detail small{
      color:var(--cream);
      letter-spacing:.18em;
      text-transform:uppercase;
      font-size:11px;
    }
    .detail strong{
      font-family:"Cormorant Garamond",serif;
      font-weight:300;
      font-style:italic;
      font-size:34px;
      line-height:1.08;
      margin:24px 0 14px;
    }
    .detail p{
      color:rgba(246,240,225,.72);
      line-height:1.75;
      font-size:15px;
    }

    .map-card{
      margin-top:18px;
      border-radius:var(--radius);
      overflow:hidden;
      border:1px solid rgba(231,216,173,.16);
      background:rgba(255,250,240,.06);
      min-height:330px;
      display:grid;
      grid-template-columns:.9fr 1.1fr;
    }
    .map-info{
      padding:34px;
      display:flex;
      flex-direction:column;
      justify-content:center;
    }
    .map-info h3{
      font-size:42px;
      font-weight:300;
      margin-bottom:14px;
    }
    .map-info p{
      color:rgba(246,240,225,.74);
      line-height:1.8;
      margin-bottom:22px;
    }
    .map-frame{
      min-height:330px;
      background:rgba(231,216,173,.12);
    }
    .map-frame iframe{
      width:100%;
      height:100%;
      border:0;
      filter:grayscale(.55) contrast(.95) sepia(.14);
    }

    .program{
      max-width:820px;
      margin:0 auto;
      display:grid;
      gap:0;
      border-top:1px solid var(--line);
    }
    .program-item{
      display:grid;
      grid-template-columns:120px 26px 1fr;
      gap:22px;
      padding:24px 0;
      border-bottom:1px solid var(--line);
      align-items:start;
    }
    .time{
      font-family:"Cormorant Garamond",serif;
      font-size:32px;
      font-style:italic;
      color:var(--wine);
      line-height:1;
    }
    .dot{
      width:13px;height:13px;border-radius:50%;
      background:var(--wine);
      margin-top:9px;
      box-shadow:0 0 0 8px rgba(101,9,27,.08);
    }
    .program-item h3{
      font-size:18px;
      font-weight:400;
      margin-bottom:7px;
    }
    .program-item p{
      color:var(--muted);
      line-height:1.7;
    }

    .dress-grid{
      display:grid;
      grid-template-columns:.9fr 1.1fr;
      gap:24px;
      align-items:stretch;
    }
    .dress-panel{
      background:rgba(255,250,240,.08);
      border:1px solid rgba(231,216,173,.16);
      border-radius:var(--radius);
      padding:34px;
    }
    .dress-panel h3{
      font-family:"Cormorant Garamond",serif;
      font-weight:300;
      font-style:italic;
      font-size:42px;
      margin-bottom:16px;
    }
    .dress-panel p{
      color:rgba(246,240,225,.74);
      line-height:1.85;
      margin-bottom:18px;
    }
    .color-list{
      display:grid;
      gap:12px;
    }
    .color-row{
      display:flex;
      align-items:center;
      gap:14px;
      padding:14px;
      border-radius:18px;
      background:rgba(255,250,240,.08);
      border:1px solid rgba(231,216,173,.13);
    }
    .color-row .swatch{width:44px;height:44px;box-shadow:none}
    .color-row span{
      color:rgba(246,240,225,.88);
      font-size:15px;
    }

    .wish{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:18px;
    }
    .wish-card{
      background:#fffaf0;
      border:1px solid var(--line);
      border-radius:var(--radius);
      padding:30px;
    }
    .wish-card h3{
      font-family:"Cormorant Garamond",serif;
      font-weight:300;
      font-style:italic;
      font-size:38px;
      margin-bottom:12px;
      color:var(--wine);
    }
    .wish-card p{
      line-height:1.85;
      color:var(--muted);
    }

    .rsvp-wrap{
      display:grid;
      grid-template-columns:.9fr 1.1fr;
      gap:24px;
      align-items:start;
    }
    .contact-card,.form-card{
      background:rgba(255,250,240,.94);
      color:var(--text);
      border:1px solid rgba(231,216,173,.24);
      border-radius:var(--radius);
      padding:34px;
      box-shadow:var(--shadow);
    }
    .contact-card h3,.form-card h3{
      font-family:"Cormorant Garamond",serif;
      font-style:italic;
      font-weight:300;
      font-size:42px;
      margin-bottom:16px;
    }
    .contact-list{display:grid;gap:12px;margin-top:22px}
    .contact-link{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:12px;
      padding:15px 16px;
      border-radius:18px;
      background:rgba(101,9,27,.06);
      border:1px solid rgba(101,9,27,.10);
      text-decoration:none;
      color:var(--text);
    }
    .contact-link span{color:var(--muted); font-size:13px}
    form{display:grid;gap:14px}
    label{
      display:grid;
      gap:7px;
      color:var(--muted);
      font-size:12px;
      letter-spacing:.12em;
      text-transform:uppercase;
    }
    input,select,textarea{
      width:100%;
      border:1px solid var(--line);
      background:#fffaf0;
      color:var(--text);
      border-radius:16px;
      padding:14px 15px;
      outline:none;
      transition:.2s ease;
      letter-spacing:normal;
      text-transform:none;
      font-size:15px;
    }
    textarea{min-height:110px;resize:vertical}
    input:focus,select:focus,textarea:focus{border-color:rgba(101,9,27,.5);box-shadow:0 0 0 4px rgba(101,9,27,.08)}
    .two{display:grid;grid-template-columns:1fr 1fr;gap:14px}
    .form-note{
      color:var(--muted);
      font-size:13px;
      line-height:1.6;
      margin-top:6px;
    }
    .success{
      display:none;
      padding:22px;
      border-radius:22px;
      background:rgba(79,75,56,.08);
      border:1px solid rgba(79,75,56,.13);
      line-height:1.7;
    }

    footer{
      padding:54px 0 100px;
      text-align:center;
      color:rgba(246,240,225,.72);
    }
    footer .script{
      display:block;
      font-size:42px;
      color:var(--cream);
      margin-bottom:10px;
    }

    @media (max-width:900px){
      .hero-inner,.map-card,.dress-grid,.wish,.rsvp-wrap{grid-template-columns:1fr}
      .hero-card{transform:none}
      .details-grid{grid-template-columns:1fr}
      .topbar{overflow:auto;justify-content:flex-start}
      .topbar::-webkit-scrollbar{display:none}
    }
    @media (max-width:640px){
      .container{width:min(100% - 22px,1120px)}
      .hero{padding:54px 0 96px}
      .hero-text{font-size:16px}
      .palette-card{min-height:450px}
      section{padding:70px 0}
      .countdown{grid-template-columns:repeat(2,1fr)}
      .program-item{grid-template-columns:82px 18px 1fr;gap:14px}
      .time{font-size:26px}
      .two{grid-template-columns:1fr}
      .contact-card,.form-card,.dress-panel,.wish-card,.detail{padding:24px}
      .topbar a{font-size:11px;padding:9px 10px}
    }
  </style>
</head>
<body>
  <nav class="topbar" aria-label="Навигация по сайту">
    <a href="#invite">Приглашение</a>
    <a href="#details">Детали</a>
    <a href="#program">Программа</a>
    <a href="#dresscode">Дресс-код</a>
    <a href="#rsvp">RSVP</a>
  </nav>

  <main class="page">
    <header class="hero" id="top">
      <div class="petals" id="petals"></div>
      <div class="container hero-inner">
        <div>
          <div class="eyebrow">Wedding invitation</div>
          <h1>
            Виталий
            <span class="amp">&</span>
            Дарья
          </h1>
          <p class="hero-text">
            Мы будем счастливы разделить с вами день, с которого начнётся наша семейная история.
            Приглашаем вас на нашу свадьбу в Самаре.
          </p>
          <div class="hero-actions">
            <a class="btn primary" href="#rsvp">Подтвердить участие</a>
            <a class="btn" target="_blank" rel="noopener" href="https://yandex.ru/maps/?text=%D0%A1%D0%B0%D0%BC%D0%B0%D1%80%D0%B0%2C%20%D0%9F%D1%80%D0%BE%D0%B3%D0%BE%D0%BD%D0%BD%D1%8B%D0%B9%20%D0%BF%D1%80%D0%BE%D0%B5%D0%B7%D0%B4%2C%206">Открыть карту</a>
          </div>
        </div>

        <aside class="hero-card" aria-label="Дата свадьбы и палитра">
          <div class="palette-card">
            <div class="date-badge">
              <span></span>
              <strong>11.09.2026</strong>
              <span></span>
            </div>
            <div class="palette">
              <i class="swatch" style="background:#050505"></i>
              <i class="swatch" style="background:#65091b"></i>
              <i class="swatch" style="background:#4f4b38"></i>
              <i class="swatch" style="background:#a18c77"></i>
              <i class="swatch" style="background:#e7d8ad"></i>
            </div>
          </div>
        </aside>
      </div>
    </header>

    <section class="section-light" id="invite">
      <div class="container">
        <div class="section-head">
          <div class="kicker">Дорогие гости</div>
          <h2>Приглашаем вас</h2>
          <p class="lead">В этот день рядом с нами хочется видеть самых близких людей.</p>
        </div>
        <div class="invite-card">
          <p>
            Совсем скоро состоится важное и радостное событие — наша свадьба.
            Мы с большой теплотой приглашаем вас разделить с нами этот особенный вечер:
            стать свидетелями начала нашей семейной жизни, порадоваться вместе с нами,
            сказать тёплые слова и сохранить в памяти атмосферу любви, света и праздника.
          </p>
          <div class="countdown" aria-label="Обратный отсчёт до свадьбы">
            <div class="cd"><div class="cd-num" id="days">—</div><div class="cd-label">дней</div></div>
            <div class="cd"><div class="cd-num" id="hours">—</div><div class="cd-label">часов</div></div>
            <div class="cd"><div class="cd-num" id="minutes">—</div><div class="cd-label">минут</div></div>
            <div class="cd"><div class="cd-num" id="seconds">—</div><div class="cd-label">секунд</div></div>
          </div>
        </div>
      </div>
    </section>

    <section class="section-dark" id="details">
      <div class="container">
        <div class="section-head">
          <div class="kicker">Где и когда</div>
          <h2>Детали праздника</h2>
          <p class="lead">Пожалуйста, сохраните дату и приезжайте немного заранее, чтобы спокойно встретиться и настроиться на вечер.</p>
        </div>

        <div class="details-grid">
          <article class="detail">
            <small>Дата</small>
            <strong>11 сентября 2026</strong>
            <p>Пятница, день нашей свадьбы.</p>
          </article>
          <article class="detail">
            <small>Время</small>
            <strong>17:00</strong>
            <p>Начало праздника. Просим гостей прибыть за 15–20 минут до начала.</p>
          </article>
          <article class="detail">
            <small>Адрес</small>
            <strong>Самара</strong>
            <p>Прогонный проезд, д. 6</p>
          </article>
        </div>

        <div class="map-card">
          <div class="map-info">
            <h3 class="script">Место встречи</h3>
            <p>
              Самара, Прогонный проезд, дом 6.
              Для удобства вы можете открыть адрес на карте и построить маршрут.
            </p>
            <a class="btn" target="_blank" rel="noopener" href="https://yandex.ru/maps/?text=%D0%A1%D0%B0%D0%BC%D0%B0%D1%80%D0%B0%2C%20%D0%9F%D1%80%D0%BE%D0%B3%D0%BE%D0%BD%D0%BD%D1%8B%D0%B9%20%D0%BF%D1%80%D0%BE%D0%B5%D0%B7%D0%B4%2C%206">Построить маршрут</a>
          </div>
          <div class="map-frame" aria-label="Карта">
            <iframe src="https://yandex.ru/map-widget/v1/?text=%D0%A1%D0%B0%D0%BC%D0%B0%D1%80%D0%B0%2C%20%D0%9F%D1%80%D0%BE%D0%B3%D0%BE%D0%BD%D0%BD%D1%8B%D0%B9%20%D0%BF%D1%80%D0%BE%D0%B5%D0%B7%D0%B4%2C%206&z=15" loading="lazy"></iframe>
          </div>
        </div>
      </div>
    </section>

    <section class="section-light" id="program">
      <div class="container">
        <div class="section-head">
          <div class="kicker">План вечера</div>
          <h2>Программа дня</h2>
          <p class="lead">Расписание можно будет уточнить ближе к дате, но общий ритм вечера будет таким.</p>
        </div>

        <div class="program">
          <div class="program-item">
            <div class="time">16:40</div>
            <div class="dot"></div>
            <div>
              <h3>Сбор гостей</h3>
              <p>Встречаемся, знакомимся, делаем первые фотографии и готовимся к началу праздника.</p>
            </div>
          </div>
          <div class="program-item">
            <div class="time">17:00</div>
            <div class="dot"></div>
            <div>
              <h3>Торжественное начало</h3>
              <p>Самый важный момент дня, который мы хотим прожить вместе с вами.</p>
            </div>
          </div>
          <div class="program-item">
            <div class="time">18:00</div>
            <div class="dot"></div>
            <div>
              <h3>Праздничный ужин</h3>
              <p>Тёплые слова, поздравления, уютная атмосфера и красивый вечер.</p>
            </div>
          </div>
          <div class="program-item">
            <div class="time">20:30</div>
            <div class="dot"></div>
            <div>
              <h3>Танцы и общение</h3>
              <p>Музыка, фотографии, весёлые моменты и воспоминания, которые останутся с нами надолго.</p>
            </div>
          </div>
          <div class="program-item">
            <div class="time">22:30</div>
            <div class="dot"></div>
            <div>
              <h3>Торт и финал вечера</h3>
              <p>Сладкое завершение праздника и благодарность каждому гостю за этот день.</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="section-dark" id="dresscode">
      <div class="container">
        <div class="section-head">
          <div class="kicker">Атмосфера</div>
          <h2>Дресс-код</h2>
          <p class="lead">Мы выбрали глубокую, благородную палитру: чёрный, винный, оливковый, тауп и мягкий беж.</p>
        </div>

        <div class="dress-grid">
          <div class="dress-panel">
            <h3>Будем рады, если вы поддержите стиль вечера</h3>
            <p>
              Для девушек подойдут вечерние или коктейльные платья в глубоких оттенках.
              Для мужчин — костюм, рубашка, тёмные или благородные натуральные тона.
            </p>
            <p>
              Просим по возможности избегать полностью белых и кремовых образов — эти оттенки оставим для невесты.
            </p>
          </div>
          <div class="dress-panel">
            <div class="color-list">
              <div class="color-row"><i class="swatch" style="background:#050505"></i><span>Чёрный — элегантная база</span></div>
              <div class="color-row"><i class="swatch" style="background:#65091b"></i><span>Винный — главный акцент</span></div>
              <div class="color-row"><i class="swatch" style="background:#4f4b38"></i><span>Оливковый — природная глубина</span></div>
              <div class="color-row"><i class="swatch" style="background:#a18c77"></i><span>Тауп — мягкий нейтральный тон</span></div>
              <div class="color-row"><i class="swatch" style="background:#e7d8ad"></i><span>Бежевый — тёплое дополнение</span></div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="section-light" id="wishes">
      <div class="container">
        <div class="section-head">
          <div class="kicker">Пожелания</div>
          <h2>Несколько важных деталей</h2>
        </div>
        <div class="wish">
          <article class="wish-card">
            <h3>Подарки</h3>
            <p>
              Ваше присутствие — самый ценный подарок для нас.
              Если вы захотите порадовать нас дополнительно, мы будем благодарны за вклад в нашу семейную мечту.
            </p>
          </article>
          <article class="wish-card">
            <h3>Цветы</h3>
            <p>
              Если вы планировали подарить букет, можно заменить его на бутылочку любимого напитка,
              книгу или другой небольшой знак внимания, который будет радовать нас дольше.
            </p>
          </article>
        </div>
      </div>
    </section>

    <section class="section-dark" id="rsvp">
      <div class="container">
        <div class="section-head">
          <div class="kicker">RSVP</div>
          <h2>Подтвердите участие</h2>
          <p class="lead">Пожалуйста, сообщите нам, сможете ли вы быть с нами в этот день.</p>
        </div>

        <div class="rsvp-wrap">
          <aside class="contact-card">
            <h3>Связаться с нами</h3>
            <p class="lead" style="color:var(--muted);font-size:16px">
              По всем вопросам можно написать или позвонить Виталию.
            </p>
            <div class="contact-list">
              <a class="contact-link" href="tel:+79083916471"><strong>Позвонить</strong><span>+7 908 391-64-71</span></a>
              <a class="contact-link" href="https://t.me/elisov_7" target="_blank" rel="noopener"><strong>Telegram</strong><span>@elisov_7</span></a>
              <a class="contact-link" href="https://vk.ru/elisov_7" target="_blank" rel="noopener"><strong>ВКонтакте</strong><span>vk.ru/elisov_7</span></a>
              <a class="contact-link" href="mailto:elisov_vitalik@mail.ru"><strong>Почта</strong><span>elisov_vitalik@mail.ru</span></a>
            </div>
          </aside>

          <div class="form-card">
            <h3>Анкета гостя</h3>
            <form id="rsvpForm">
              <label>
                Ваше имя и фамилия
                <input id="guestName" required placeholder="Например: Иван Иванов" />
              </label>

              <div class="two">
                <label>
                  Присутствие
                  <select id="attendance" required>
                    <option value="">Выберите...</option>
                    <option value="Приду с радостью">Приду с радостью</option>
                    <option value="К сожалению, не смогу">К сожалению, не смогу</option>
                  </select>
                </label>
                <label>
                  Количество гостей
                  <select id="guestCount">
                    <option>1</option>
                    <option>2</option>
                    <option>3</option>
                    <option>4</option>
                  </select>
                </label>
              </div>

              <label>
                Пожелания / аллергии / комментарий
                <textarea id="comment" placeholder="Напишите, если есть важные пожелания"></textarea>
              </label>

              <button class="btn dark" type="submit">Сформировать ответ</button>
              <p class="form-note">
                После отправки появятся кнопки для связи: можно отправить готовый текст в Telegram, WhatsApp или на почту.
              </p>

              <div class="success" id="successBox">
                <strong>Спасибо! Ответ сформирован.</strong>
                <p id="messagePreview" style="margin:12px 0"></p>
                <div class="hero-actions" style="margin-top:14px">
                  <a class="btn primary" id="tgLink" target="_blank" rel="noopener">Отправить в Telegram</a>
                  <a class="btn light" id="waLink" target="_blank" rel="noopener">WhatsApp</a>
                  <a class="btn light" id="mailLink">Email</a>
                </div>
              </div>
            </form>
          </div>
        </div>
      </div>
    </section>

    <footer>
      <div class="container">
        <span class="script">Виталий & Дарья</span>
        <p>11 сентября 2026 · Самара</p>
      </div>
    </footer>
  </main>

  <script>
    const weddingDate = new Date("2026-09-11T17:00:00+04:00");

    function pad(n){ return String(n).padStart(2,"0"); }

    function updateCountdown(){
      const now = new Date();
      let diff = weddingDate - now;
      if(diff < 0) diff = 0;

      const days = Math.floor(diff / 86400000);
      const hours = Math.floor((diff % 86400000) / 3600000);
      const minutes = Math.floor((diff % 3600000) / 60000);
      const seconds = Math.floor((diff % 60000) / 1000);

      document.getElementById("days").textContent = days;
      document.getElementById("hours").textContent = pad(hours);
      document.getElementById("minutes").textContent = pad(minutes);
      document.getElementById("seconds").textContent = pad(seconds);
    }
    updateCountdown();
    setInterval(updateCountdown, 1000);

    function spawnPetals(){
      const container = document.getElementById("petals");
      const colors = ["#65091b","#a18c77","#e7d8ad","#4f4b38","#3c040f"];
      for(let i=0;i<32;i++){
        const p = document.createElement("i");
        p.className = "petal";
        p.style.left = Math.random() * 100 + "%";
        p.style.animationDuration = (8 + Math.random() * 12) + "s";
        p.style.animationDelay = (Math.random() * 12) + "s";
        p.style.background = colors[Math.floor(Math.random()*colors.length)];
        p.style.transform = "rotate(" + Math.random()*180 + "deg)";
        container.appendChild(p);
      }
    }
    spawnPetals();

    document.getElementById("rsvpForm").addEventListener("submit", function(e){
      e.preventDefault();

      const name = document.getElementById("guestName").value.trim();
      const attendance = document.getElementById("attendance").value;
      const guestCount = document.getElementById("guestCount").value;
      const comment = document.getElementById("comment").value.trim();

      if(!name || !attendance) return;

      const text =
        "Здравствуйте! Это ответ на свадебное приглашение Виталия и Дарьи.%0A%0A" +
        "Имя: " + encodeURIComponent(name) + "%0A" +
        "Присутствие: " + encodeURIComponent(attendance) + "%0A" +
        "Количество гостей: " + encodeURIComponent(guestCount) + "%0A" +
        "Комментарий: " + encodeURIComponent(comment || "нет");

      const readable =
        "Имя: " + name + "\\n" +
        "Присутствие: " + attendance + "\\n" +
        "Количество гостей: " + guestCount + "\\n" +
        "Комментарий: " + (comment || "нет");

      document.getElementById("messagePreview").textContent = readable;
      document.getElementById("tgLink").href = "https://t.me/elisov_7";
      document.getElementById("waLink").href = "https://wa.me/79083916471?text=" + text;
      document.getElementById("mailLink").href =
        "mailto:elisov_vitalik@mail.ru?subject=" +
        encodeURIComponent("RSVP на свадьбу Виталия и Дарьи") +
        "&body=" + text.replaceAll("%0A", "%0D%0A");

      document.getElementById("successBox").style.display = "block";
      document.getElementById("successBox").scrollIntoView({behavior:"smooth", block:"center"});
    });
  </script>
</body>
</html>
