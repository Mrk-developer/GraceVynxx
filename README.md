<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <meta
    name="description"
    content="GraceVynx Virtual Assistant — Social Media Management, Lead Generation, Email Marketing, and administrative support for growing businesses."
  />

  <title>GraceVynx | Virtual Assistant</title>

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link
    href="https://fonts.googleapis.com/css2?family=League+Spartan:wght@400;500;600;700;800&family=Roboto:wght@400;500;700&display=swap"
    rel="stylesheet"
  >

  <style>
    :root {
      --purple: #A07BE6;
      --purple-dark: #7650C4;
      --purple-soft: #F0EAFE;
      --bg: #F9F9F9;
      --white: #FFFFFF;
      --text: #272331;
      --muted: #6F687A;
      --border: #E7E1F2;
      --shadow: 0 22px 60px rgba(70,43,117,.12);
      --radius: 24px;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Roboto', sans-serif;
      color: var(--text);
      background: var(--bg);
      line-height: 1.7;
    }

    a {
      color: inherit;
      text-decoration: none;
    }

    img {
      max-width: 100%;
      display: block;
    }

    button,
    input,
    textarea {
      font: inherit;
    }

    .container {
      width: min(1160px, 92%);
      margin-inline: auto;
    }

    header {
      position: fixed;
      inset: 0 0 auto 0;
      z-index: 1000;
      background: rgba(249,249,249,.92);
      backdrop-filter: blur(16px);
      border-bottom: 1px solid rgba(160,123,230,.14);
    }

    .nav {
      min-height: 78px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 20px;
    }

    .brand {
      font-family: 'League Spartan', sans-serif;
      font-size: 1.55rem;
      font-weight: 800;
      letter-spacing: -.04em;
      color: var(--text);
    }

    .brand span {
      color: var(--purple);
    }

    .brand-text {
      font-family: 'League Spartan', sans-serif;
      font-size: 1.55rem;
      font-weight: 800;
      letter-spacing: -.04em;
      color: var(--text);
    }

    .brand-text span {
      color: var(--purple);
    }

    .nav-links {
      display: flex;
      align-items: center;
      gap: 28px;
      list-style: none;
    }

    .nav-links a {
      font-size: .92rem;
      font-weight: 600;
      color: #4F485B;
      transition: .25s ease;
    }

    .nav-links a:hover {
      color: var(--purple-dark);
    }

    .nav-cta {
      background: var(--purple);
      color: #fff !important;
      padding: 10px 18px;
      border-radius: 999px;
      box-shadow: 0 8px 20px rgba(160,123,230,.25);
    }

    .nav-toggle {
      display: none;
      border: 0;
      background: transparent;
      font-size: 1.7rem;
      color: var(--purple-dark);
      cursor: pointer;
    }

    .hero {
      padding: 150px 0 105px;
      overflow: hidden;
      min-height: 760px;
      display: flex;
      align-items: center;
    }

    .hero-grid {
      display: grid;
      grid-template-columns: 1.02fr .98fr;
      align-items: center;
      gap: 70px;
    }

    .eyebrow {
      display: inline-flex;
      align-items: center;
      gap: 8px;
      color: var(--purple-dark);
      background: var(--purple-soft);
      padding: 7px 13px;
      border-radius: 999px;
      font-size: .78rem;
      font-weight: 800;
      text-transform: uppercase;
      letter-spacing: .12em;
      margin-bottom: 20px;
    }

    .hero h1 {
      font-family: 'League Spartan', sans-serif;
      font-size: clamp(3rem,6vw,5.4rem);
      line-height: .94;
      letter-spacing: -.05em;
      margin-bottom: 24px;
      max-width: 760px;
    }

    .hero h1 span {
      color: var(--purple);
    }

    .hero h2 {
      font-family: 'League Spartan', sans-serif;
      font-size: clamp(1.35rem,2vw,1.8rem);
      line-height: 1.15;
      margin-bottom: 18px;
      color: #40384D;
    }

    .hero p {
      color: var(--muted);
      max-width: 680px;
      font-size: 1.05rem;
    }

    .hero-buttons {
      display: flex;
      flex-wrap: wrap;
      gap: 13px;
      margin-top: 30px;
    }

    .btn {
      display: inline-flex;
      justify-content: center;
      align-items: center;
      gap: 8px;
      padding: 14px 22px;
      border-radius: 12px;
      border: 1px solid transparent;
      font-weight: 700;
      transition:
        transform .2s ease,
        box-shadow .2s ease,
        background .2s ease;
      cursor: pointer;
    }

    .btn:hover {
      transform: translateY(-2px);
    }

    .btn-primary {
      background: var(--purple);
      color: #fff;
      box-shadow: 0 12px 25px rgba(160,123,230,.28);
    }

    .btn-secondary {
      background: #fff;
      border-color: var(--border);
      color: var(--text);
    }

    .hero-visual {
      position: relative;
      min-height: 600px;
      display: grid;
      place-items: center;
    }

    .photo-wrap {
      width: min(465px,90%);
      height: 560px;
      position: relative;
      z-index: 2;
      border-radius: 48% 48% 28% 28% / 38% 38% 18% 18%;
      background: linear-gradient(145deg,#EEE7FF,#fff);
      padding: 14px;
      box-shadow: var(--shadow);
      transform: rotate(2deg);
    }

    .photo-wrap::before {
      content: '';
      position: absolute;
      inset: 14px;
      border-radius: inherit;
      background: #EDE6FA;
      z-index: -1;
    }

    .photo-wrap img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center top;
      border-radius: inherit;
      transform: rotate(-2deg);
    }

    .photo-ring {
      position: absolute;
      width: 520px;
      height: 520px;
      border: 1px solid rgba(160,123,230,.25);
      border-radius: 50%;
      right: 0;
      top: 40px;
      z-index: 0;
    }

    .photo-dot {
      position: absolute;
      width: 125px;
      height: 125px;
      border-radius: 50%;
      background: rgba(160,123,230,.13);
      right: -5px;
      bottom: 55px;
      z-index: 1;
    }

    .photo-dot.small {
      width: 62px;
      height: 62px;
      left: 10px;
      top: 80px;
      right: auto;
      bottom: auto;
      background: rgba(160,123,230,.18);
    }

    .floating {
      position: absolute;
      z-index: 4;
      background: #fff;
      border: 1px solid var(--border);
      box-shadow: var(--shadow);
      padding: 12px 16px;
      border-radius: 15px;
      font-weight: 700;
      font-size: .86rem;
    }

    .float-one {
      top: 18%;
      left: 0;
    }

    .float-two {
      right: 0;
      bottom: 16%;
    }

    .photo-caption {
      position: absolute;
      left: 50%;
      bottom: -10px;
      transform: translateX(-50%);
      z-index: 4;
      background: var(--text);
      color: #fff;
      padding: 9px 17px;
      border-radius: 999px;
      font-size: .8rem;
      font-weight: 700;
      white-space: nowrap;
      box-shadow: 0 10px 25px rgba(39,35,49,.18);
    }

    section {
      padding: 92px 0;
    }

    .section-head {
      text-align: center;
      max-width: 720px;
      margin: 0 auto 48px;
    }

    .section-kicker {
      color: var(--purple-dark);
      font-size: .78rem;
      text-transform: uppercase;
      letter-spacing: .14em;
      font-weight: 800;
      margin-bottom: 9px;
    }

    .section-head h2 {
      font-family: 'League Spartan', sans-serif;
      font-size: clamp(2.3rem,4vw,3.4rem);
      line-height: 1;
      margin-bottom: 14px;
    }

    .section-head p {
      color: var(--muted);
    }


    .services {
      background: #fff;
    }

    .service-grid {
      display: grid;
      grid-template-columns: repeat(3,1fr);
      gap: 22px;
    }

    .service-card {
      padding: 32px;
      background: var(--bg);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      transition: .25s ease;
      position: relative;
      overflow: hidden;
    }

    .service-card:hover {
      transform: translateY(-6px);
      box-shadow: var(--shadow);
      border-color: rgba(160,123,230,.4);
    }

    .service-icon {
      width: 54px;
      height: 54px;
      display: grid;
      place-items: center;
      border-radius: 15px;
      background: var(--purple);
      color: #fff;
      font-size: 1.55rem;
      margin-bottom: 21px;
    }

    .service-card h3 {
      font-family: 'League Spartan', sans-serif;
      font-size: 1.65rem;
      margin-bottom: 9px;
    }

    .service-card p {
      color: var(--muted);
      margin-bottom: 18px;
    }

    .service-card ul,
    .expect-list {
      list-style: none;
    }

    .service-card li {
      margin: 7px 0;
      font-size: .94rem;
    }

    .service-card li::before {
      content: '✓';
      color: var(--purple);
      font-weight: 900;
      margin-right: 9px;
    }

    .expect-grid {
      display: grid;
      grid-template-columns: .85fr 1.15fr;
      gap: 55px;
      align-items: center;
    }

    .expect-panel {
      background: var(--purple);
      color: #fff;
      border-radius: 32px;
      padding: 45px;
      position: relative;
      overflow: hidden;
    }

    .expect-panel::after {
      content: 'GV';
      position: absolute;
      right: -20px;
      bottom: -70px;
      font-family: 'League Spartan';
      font-size: 12rem;
      font-weight: 800;
      opacity: .09;
    }

    .expect-panel h3 {
      font-family: 'League Spartan';
      font-size: 2.7rem;
      line-height: 1;
      margin-bottom: 15px;
      position: relative;
      z-index: 1;
    }

    .expect-panel p {
      opacity: .9;
      position: relative;
      z-index: 1;
    }

    .expect-list {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 15px;
    }

    .expect-list li {
      background: #fff;
      border: 1px solid var(--border);
      border-radius: 15px;
      padding: 16px;
      font-weight: 600;
      box-shadow: 0 8px 25px rgba(50,30,90,.04);
    }

    .expect-list li span {
      color: var(--purple);
      margin-right: 7px;
    }

    .portfolio {
      background: #fff;
    }

    .portfolio-box {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 30px;
      align-items: stretch;
    }

    .portfolio-copy {
      padding: 45px;
      border-radius: 30px;
      background: var(--purple-soft);
    }

    .portfolio-copy h3 {
      font-family: 'League Spartan';
      font-size: 2.7rem;
      line-height: 1;
      margin-bottom: 17px;
    }

    .portfolio-copy p {
      color: var(--muted);
      margin-bottom: 20px;
    }

    .portfolio-tags {
      display: flex;
      flex-wrap: wrap;
      gap: 8px;
      margin: 22px 0 28px;
    }

    .tag {
      padding: 8px 11px;
      background: #fff;
      border: 1px solid var(--border);
      border-radius: 999px;
      font-size: .82rem;
      font-weight: 700;
    }

    .portfolio-image {
      min-height: 370px;
      border-radius: 30px;
      overflow: hidden;
      position: relative;
      background: #eee7ff;
      display: grid;
      place-items: center;
    }

    .portfolio-image::before {
      content: 'GraceVynx';
      position: absolute;
      inset: auto 25px 22px auto;
      color: rgba(118,80,196,.16);
      font-family: 'League Spartan';
      font-size: 3.5rem;
      font-weight: 800;
    }

    .portfolio-image img {
      width: 72%;
      height: 88%;
      object-fit: cover;
      object-position: center top;
      border-radius: 22px;
      box-shadow: 0 15px 40px rgba(70,43,117,.15);
    }

    .why-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 25px;
    }

    .why-card {
      padding: 35px;
      background: #fff;
      border: 1px solid var(--border);
      border-radius: 25px;
    }

    .why-card h3 {
      font-family: 'League Spartan';
      font-size: 1.9rem;
      margin-bottom: 10px;
    }

    .steps {
      display: grid;
      gap: 13px;
    }

    .step {
      display: flex;
      align-items: center;
      gap: 14px;
      padding: 16px;
      border-radius: 15px;
      background: var(--bg);
    }

    .step-number {
      width: 38px;
      height: 38px;
      border-radius: 50%;
      display: grid;
      place-items: center;
      flex: 0 0 38px;
      background: var(--purple);
      color: #fff;
      font-weight: 800;
    }

    .about-photo {
      display: grid !important;
      grid-template-columns: 140px 1fr;
      gap: 22px;
      align-items: center;
      text-align: left !important;
      background: linear-gradient(145deg,#fff,#f0eafe) !important;
    }

    .about-photo img {
      width: 140px;
      height: 180px;
      object-fit: cover;
      object-position: center top;
      border-radius: 70px 70px 22px 22px;
      box-shadow: var(--shadow);
    }

    .cta {
      padding-top: 35px;
    }

    .cta-box {
      background: var(--text);
      color: #fff;
      border-radius: 35px;
      padding: 65px 45px;
      text-align: center;
      position: relative;
      overflow: hidden;
    }

    .cta-box::before {
      content: '';
      position: absolute;
      width: 300px;
      height: 300px;
      border: 70px solid rgba(160,123,230,.15);
      border-radius: 50%;
      top: -190px;
      left: -70px;
    }

    .cta-box h2 {
      font-family: 'League Spartan';
      font-size: clamp(2.5rem,5vw,4.3rem);
      line-height: .95;
      margin-bottom: 15px;
      position: relative;
    }

    .cta-box p {
      color: #D9D2E5;
      max-width: 650px;
      margin: 0 auto 25px;
      position: relative;
    }

    .cta-box .btn {
      position: relative;
    }

    footer {
      padding: 35px 0 45px;
    }

    .footer-inner {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 20px;
      padding-top: 28px;
      border-top: 1px solid var(--border);
    }

    .footer-inner p {
      color: var(--muted);
      font-size: .88rem;
    }

    .footer-link {
      color: var(--purple-dark);
      font-weight: 700;
    }

    .reveal {
      opacity: 0;
      transform: translateY(22px);
      transition:
        opacity .7s ease,
        transform .7s ease;
    }

    .reveal.show {
      opacity: 1;
      transform: none;
    }

    @media(max-width:850px) {

      .nav-toggle {
        display: block;
      }

      .nav-links {
        display: none;
        position: absolute;
        top: 78px;
        left: 0;
        right: 0;
        padding: 20px 5%;
        background: rgba(249,249,249,.98);
        border-bottom: 1px solid var(--border);
        flex-direction: column;
        align-items: stretch;
      }

      .nav-links.open {
        display: flex;
      }

      .nav-links a {
        display: block;
        padding: 10px 0;
      }

      .hero {
        padding-top: 125px;
        min-height: auto;
      }

      .hero-grid,
      .expect-grid,
      .portfolio-box,
      .why-grid {
        grid-template-columns: 1fr;
      }

      .hero-visual {
        order: -1;
        min-height: 520px;
      }

      .photo-wrap {
        height: 500px;
        width: min(410px,84%);
      }

      .photo-ring {
        width: 450px;
        height: 450px;
        right: 2%;
        top: 25px;
      }

      .float-one {
        left: 4%;
      }

      .float-two {
        right: 4%;
      }

      .service-grid {
        grid-template-columns: 1fr;
      }

      .about-photo {
        grid-template-columns: 1fr;
        text-align: center !important;
      }

      .about-photo img {
        margin: 0 auto;
      }
    }
    
    @media(max-width:560px) {

      section {
        padding: 70px 0;
      }

      .hero {
        padding-bottom: 60px;
      }

      .hero h1 {
        font-size: 3rem;
      }

      .hero-buttons .btn {
        width: 100%;
      }

      .expect-list {
        grid-template-columns: 1fr;
      }

      .expect-panel,
      .portfolio-copy,
      .cta-box {
        padding: 32px 24px;
      }

      .portfolio-image {
        min-height: 330px;
      }

      .photo-wrap {
        height: 420px;
      }

      .hero-visual {
        min-height: 450px;
      }

      .photo-ring {
        width: 360px;
        height: 360px;
      }

      .floating {
        font-size: .75rem;
        padding: 10px 12px;
      }

      .photo-caption {
        font-size: .72rem;
      }

      .footer-inner {
        flex-direction: column;
        text-align: center;
      }
    }
  </style>
</head>

<body>

  <header>
    <div class="container nav">

      <a href="#home" class="brand" aria-label="GraceVynx home">
        <span class="brand-text">
          Grace<span>Vynx</span>
        </span>
      </a>

      <button
        class="nav-toggle"
        aria-label="Open navigation"
        aria-expanded="false"
      >
        ☰
      </button>

      <nav>
        <ul class="nav-links" id="navLinks">

          <li>
            <a href="#home">Home</a>
          </li>

          <li>
            <a href="#services">Services</a>
          </li>

          <li>
            <a href="#portfolio">Portfolio</a>
          </li>

          <li>
            <a href="#why">Why Me</a>
          </li>

          <li>
            <a
              class="nav-cta"
              href="https://preview.mailerlite.io/forms/2659539/199553809011180889/share"
            >
              Let's Work Together
            </a>
          </li>

        </ul>
      </nav>

    </div>
  </header>

  <main>

    <!-- HERO -->
    <section class="hero" id="home">

      <div class="container hero-grid">

        <div class="reveal">

          <div class="eyebrow">
            GraceVynx • Virtual Assistant
          </div>

          <h1>
            More Time for Your Business.
            <span>Less Time on the Busywork.</span>
          </h1>

          <h2>
            Reliable Virtual Assistant Support for Your Growing Business
          </h2>

          <p>
            Running a business takes time, energy, and attention.
            From managing your social media to finding potential clients
            and keeping your audience engaged, the daily tasks can quickly pile up.
          </p>

          <p style="margin-top:14px;">
            That’s where I come in. I’m
            <strong>Grace, a Freelance Virtual Assistant</strong>
            helping entrepreneurs and small businesses stay organized,
            visible, and connected through reliable
            <strong>Social Media Management, Lead Generation, and Email Marketing</strong>
            support.
          </p>

          <div class="hero-buttons">

            <a
              class="btn btn-primary"
              href="https://preview.mailerlite.io/forms/2659539/199553809011180889/share"
            >
              Let's Work Together →
            </a>

            <a
              class="btn btn-secondary"
              href="#services"
            >
              Explore Services
            </a>

          </div>

        </div>


        <!-- HERO IMAGE -->

        <div class="hero-visual reveal">

          <div class="photo-ring"></div>

          <div class="photo-dot"></div>

          <div class="photo-dot small"></div>

          <div class="photo-wrap">

            <img
              src="grace.jpg"
              alt="Grace, Freelance Virtual Assistant"
            >

          </div>

          <div class="floating float-one">
            ✓ Reliable support
          </div>

          <div class="floating float-two">
            ✦ Organized workflow
          </div>

          <div class="photo-caption">
            Grace • Freelance Virtual Assistant
          </div>

        </div>

      </div>

    </section>

    <section class="services" id="services">

      <div class="container">

        <div class="section-head reveal">

          <div class="section-kicker">
            What I Offer
          </div>

          <h2>
            Support that keeps your business moving.
          </h2>

          <p>
            Practical, organized assistance for the tasks
            that take time away from your bigger goals.
          </p>

        </div>


        <div class="service-grid">


          <article class="service-card reveal">

            <div class="service-icon">
              📱
            </div>

            <h3>
              Social Media Management
            </h3>

            <p>
              Build a consistent online presence without spending
              hours managing your platforms.
            </p>

            <ul>

              <li>Content planning</li>
              <li>Caption creation</li>
              <li>Content scheduling</li>
              <li>Social media organization</li>
              <li>Engagement support</li>
              <li>Basic content research</li>

            </ul>

          </article>


          <!-- SERVICE 2 -->

          <article class="service-card reveal">

            <div class="service-icon">
              🎯
            </div>

            <h3>
              Lead Generation
            </h3>

            <p>
              Spend less time searching and more time connecting
              with potential clients.
            </p>

            <ul>

              <li>Prospect research</li>
              <li>Lead list building</li>
              <li>Data collection</li>
              <li>Contact research</li>
              <li>Lead organization</li>
              <li>Target audience research</li>

            </ul>

          </article>


          <!-- SERVICE 3 -->

          <article class="service-card reveal">

            <div class="service-icon">
              📧
            </div>

            <h3>
              Email Marketing
            </h3>

            <p>
              Stay connected with your audience through thoughtful
              and engaging email campaigns.
            </p>

            <ul>

              <li>Email campaign support</li>
              <li>Email copy assistance</li>
              <li>Campaign scheduling</li>
              <li>Audience/list organization</li>
              <li>Newsletter support</li>
              <li>Basic campaign research</li>

            </ul>

          </article>

        </div>

      </div>

    </section>

    <section id="expectations">

      <div class="container expect-grid">


        <div class="expect-panel reveal">

          <h3>
            More than task support.
          </h3>

          <p>
            When you work with me, you get a reliable partner
            who cares about helping your business stay organized
            and consistent.
          </p>

        </div>


        <div class="reveal">

          <div class="section-kicker">
            What You Can Expect
          </div>

          <h2
            style="
              font-family:'League Spartan';
              font-size:clamp(2.3rem,4vw,3.5rem);
              line-height:1;
              margin-bottom:18px;
            "
          >
            A dependable extra set of hands.
          </h2>

          <ul class="expect-list">

            <li>
              <span>✔</span>
              Reliable and professional support
            </li>

            <li>
              <span>✔</span>
              Detail-oriented work
            </li>

            <li>
              <span>✔</span>
              Clear communication
            </li>

            <li>
              <span>✔</span>
              Organized workflow
            </li>

            <li>
              <span>✔</span>
              Personalized assistance
            </li>

            <li>
              <span>✔</span>
              More time to focus on your business
            </li>

          </ul>

        </div>

      </div>

    </section>


    <!-- =========================
         PORTFOLIO
    ========================= -->

    <section class="portfolio" id="portfolio">

      <div class="container">

        <div class="section-head reveal">

          <div class="section-kicker">
            My Portfolio
          </div>

          <h2>
            See my work in action.
          </h2>

          <p>
            Explore examples of my work and get a closer look
            at my skills, creativity, and attention to detail.
          </p>

        </div>


        <div class="portfolio-box">


          <div class="portfolio-copy reveal">

            <h3>
              Let the work speak for itself.
            </h3>

            <p>
              From content planning and social media posts to
              lead research and email campaigns, my portfolio
              shows how I can support your business behind the scenes.
            </p>


            <div class="portfolio-tags">

              <span class="tag">
                Social Media
              </span>

              <span class="tag">
                Lead Generation
              </span>

              <span class="tag">
                Email Marketing
              </span>

              <span class="tag">
                Administrative Support
              </span>

            </div>


            <a
              class="btn btn-primary"
              href="https://linktr.ee/gracevynx"
              target="_blank"
              rel="noopener"
            >
              View My Portfolio ↗
            </a>

          </div>


          <div class="portfolio-image reveal">

            <img
              src="gracee.png"
              alt="GraceVynx portfolio portrait"
            >

          </div>

        </div>

      </div>

    </section>


    <!-- =========================
         WHY ME
    ========================= -->

    <section id="why">

      <div class="container">

        <div class="section-head reveal">

          <div class="section-kicker">
            Why Work With Me?
          </div>

          <h2>
            Simple support. Clear process.
          </h2>

          <p>
            Every business has different goals, challenges,
            and priorities. I take the time to understand what
            you need and provide support that fits your workflow.
          </p>

        </div>


        <div class="why-grid">


          <!-- APPROACH -->

          <div class="why-card reveal">

            <h3>
              My approach
            </h3>

            <p
              style="
                color:var(--muted);
                margin-bottom:20px;
              "
            >
              Whether you need help maintaining your online presence,
              finding potential leads, or staying connected with your
              audience, I’m here to make your workload more manageable.
            </p>


            <div class="steps">

              <div class="step">

                <span class="step-number">
                  1
                </span>

                <strong>
                  Listen
                </strong>

              </div>


              <div class="step">

                <span class="step-number">
                  2
                </span>

                <strong>
                  Organize
                </strong>

              </div>


              <div class="step">

                <span class="step-number">
                  3
                </span>

                <strong>
                  Support
                </strong>

              </div>


              <div class="step">

                <span class="step-number">
                  4
                </span>

                <strong>
                  Deliver
                </strong>

              </div>

            </div>

          </div>


          <!-- ABOUT -->

          <div class="why-card reveal about-photo">

            <img
              src="graceee.png"
              alt="Grace, Freelance Virtual Assistant"
            >

            <div>

              <h3>
                Hi, I’m Grace.
              </h3>

              <p
                style="color:var(--muted);"
              >
                Helping entrepreneurs and small businesses
                stay organized, visible, and connected through
                dependable virtual support.
              </p>

            </div>

          </div>

        </div>

      </div>

    </section>


    <!-- =========================
         CALL TO ACTION
    ========================= -->

    <section class="cta">

      <div class="container">

        <div class="cta-box reveal">

          <h2>
            Ready to Get More Done?
          </h2>

          <p>
            You don't have to handle everything on your own.
            Let’s work together to simplify your workload,
            stay consistent, and give you more time to focus
            on growing your business.
          </p>

          <a
            class="btn btn-primary"
            href="https://preview.mailerlite.io/forms/2659539/199553809011180889/share"
          >
            Let's Work Together ↗
          </a>

          <p
            style="
              margin-top:14px;
              margin-bottom:0;
              font-size:.9rem;
            "
          >
            Have a project in mind? Let’s talk.
          </p>

        </div>

      </div>

    </section>

  </main>


  <!-- =========================
       FOOTER
  ========================= -->

  <footer>

    <div class="container footer-inner">

      <span class="brand-text">
        Grace<span>Vynx</span>
      </span>

      <p>
        © <span id="year"></span>
        GraceVynx. All rights reserved.
      </p>

      <a
        class="footer-link"
        href="https://linktr.ee/gracevynx"
        target="_blank"
        rel="noopener"
      >
        linktr.ee/gracevynx ↗
      </a>

    </div>

  </footer>


  <!-- =========================
       JAVASCRIPT
  ========================= -->

  <script>

    /* =========================
       MOBILE NAVIGATION
    ========================= */

    const toggle =
      document.querySelector('.nav-toggle');

    const navLinks =
      document.querySelector('#navLinks');


    toggle.addEventListener('click', () => {

      const open =
        navLinks.classList.toggle('open');

      toggle.setAttribute(
        'aria-expanded',
        open
      );

      toggle.textContent =
        open ? '✕' : '☰';

    });


    /* CLOSE MOBILE MENU
       AFTER CLICKING A LINK
    */

    document
      .querySelectorAll('#navLinks a')
      .forEach(link => {

        link.addEventListener('click', () => {

          navLinks.classList.remove('open');

          toggle.setAttribute(
            'aria-expanded',
            'false'
          );

          toggle.textContent = '☰';

        });

      });


    /* =========================
       SCROLL REVEAL ANIMATION
    ========================= */

    const observer =
      new IntersectionObserver(
        (entries) => {

          entries.forEach(entry => {

            if (entry.isIntersecting) {

              entry.target.classList.add('show');

              observer.unobserve(
                entry.target
              );

            }

          });

        },
        {
          threshold: 0.12
        }
      );


    document
      .querySelectorAll('.reveal')
      .forEach(el => {

        observer.observe(el);

      });


    /* =========================
       CURRENT YEAR
    ========================= */

    document.getElementById('year').textContent =
      new Date().getFullYear();

  </script>

</body>
</html>
