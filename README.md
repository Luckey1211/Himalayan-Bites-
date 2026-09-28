# Himalayan-Bites-
Organic snacks 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="theme-color" content="#183d2a">
  <meta name="description" content="Discover Himalayan Bites Ghugute—a traditional Uttarakhand treat made with whole wheat and jaggery.">
  <title>Himalayan Bites | A Taste of Uttarakhand</title>

  <style>
    :root {
      --forest: #183d2a;
      --forest-light: #28583b;
      --leaf: #77965b;
      --cream: #f8f5ed;
      --paper: #fffdf8;
      --ink: #26342b;
      --muted: #68736a;
      --line: #e8e4d9;
      --gold: #c79448;
      --content: 1160px;
      --serif: Georgia, "Times New Roman", serif;
      --sans: "Helvetica Neue", Arial, sans-serif;
    }

    *,
    *::before,
    *::after {
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
      scroll-padding-top: 6rem;
    }

    body {
      margin: 0;
      background: var(--paper);
      color: var(--ink);
      font-family: var(--sans);
      line-height: 1.65;
    }

    img {
      display: block;
      max-width: 100%;
    }

    a {
      color: inherit;
    }

    a:focus-visible,
    summary:focus-visible {
      outline: 3px solid var(--gold);
      outline-offset: 4px;
      border-radius: 3px;
    }

    .container {
      width: min(var(--content), calc(100% - 3rem));
      margin-inline: auto;
    }

    .eyebrow {
      margin: 0 0 0.75rem;
      color: var(--leaf);
      font-size: 0.75rem;
      font-weight: 700;
      letter-spacing: 0.16em;
      text-transform: uppercase;
    }

    .section-title {
      margin: 0;
      color: var(--forest);
      font: 700 clamp(2rem, 4vw, 3.2rem)/1.12 var(--serif);
      letter-spacing: -0.025em;
      text-wrap: balance;
    }

    .section-intro {
      max-width: 640px;
      margin: 1rem auto 0;
      color: var(--muted);
      font-size: 1.05rem;
    }

    .section-header {
      margin-bottom: 3rem;
      text-align: center;
    }

    .button {
      display: inline-flex;
      min-height: 3.25rem;
      align-items: center;
      justify-content: center;
      gap: 0.55rem;
      padding: 0.85rem 1.35rem;
      border: 1px solid transparent;
      border-radius: 3px;
      background: var(--forest);
      color: white;
      font-size: 0.92rem;
      font-weight: 700;
      text-decoration: none;
      transition: background-color 180ms ease, transform 180ms ease;
    }

    .button:hover {
      transform: translateY(-2px);
      background: var(--forest-light);
    }

    .button--light {
      border-color: rgba(255, 255, 255, 0.7);
      background: transparent;
    }

    .button--light:hover {
      background: rgba(255, 255, 255, 0.12);
    }

    /* Navigation */
    .site-header {
      position: sticky;
      z-index: 10;
      top: 0;
      border-bottom: 1px solid rgba(24, 61, 42, 0.08);
      background: rgba(255, 253, 248, 0.96);
      backdrop-filter: blur(12px);
    }

    .header-inner {
      display: flex;
      min-height: 76px;
      align-items: center;
      justify-content: space-between;
      gap: 2rem;
    }

    .brand {
      display: inline-flex;
      align-items: center;
      gap: 0.7rem;
      color: var(--forest);
      font: 700 1.2rem/1 var(--serif);
      text-decoration: none;
      white-space: nowrap;
    }

    .brand-mark {
      display: grid;
      width: 2.4rem;
      height: 2.4rem;
      place-items: center;
      border-radius: 50%;
      background: var(--forest);
      color: white;
      font: 700 0.9rem/1 var(--sans);
      letter-spacing: 0.04em;
    }

    .main-nav {
      display: flex;
      align-items: center;
      gap: clamp(1rem, 2.4vw, 2rem);
    }

    .main-nav a {
      color: var(--ink);
      font-size: 0.88rem;
      font-weight: 600;
      text-decoration: none;
      transition: color 180ms ease;
    }

    .main-nav a:hover {
      color: var(--leaf);
    }

    .main-nav .nav-cta {
      padding: 0.65rem 1rem;
      border-radius: 3px;
      background: var(--forest);
      color: white;
    }

    .main-nav .nav-cta:hover {
      background: var(--forest-light);
      color: white;
    }

    /* Hero */
    .hero {
      position: relative;
      display: flex;
      min-height: min(720px, calc(100svh - 76px));
      align-items: center;
      overflow: hidden;
      background:
        linear-gradient(90deg, rgba(13, 35, 23, 0.83), rgba(13, 35, 23, 0.34)),
        url("mountain-meadow.jpg") center 55% / cover no-repeat,
        #344b39;
      color: white;
    }

    .hero-content {
      width: min(700px, 100%);
      padding-block: 6rem;
    }

    .hero .eyebrow {
      color: #d9c28f;
    }

    .hero h1 {
      max-width: 700px;
      margin: 0;
      font: 700 clamp(3rem, 8vw, 6.2rem)/0.98 var(--serif);
      letter-spacing: -0.04em;
      text-wrap: balance;
    }

    .hero-copy {
      max-width: 540px;
      margin: 1.5rem 0 2rem;
      color: rgba(255, 255, 255, 0.9);
      font-size: clamp(1.05rem, 2vw, 1.25rem);
    }

    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 0.85rem;
    }

    .hero-note {
      margin: 2.5rem 0 0;
      color: rgba(255, 255, 255, 0.78);
      font-size: 0.82rem;
      letter-spacing: 0.04em;
    }

    /* Brand promise strip */
    .promise-strip {
      border-bottom: 1px solid var(--line);
      background: var(--paper);
    }

    .promise-inner {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      padding-block: 1.3rem;
    }

    .promise-item {
      padding: 0.5rem 1rem;
      color: var(--forest);
      text-align: center;
      font-size: 0.88rem;
      font-weight: 700;
    }

    .promise-item + .promise-item {
      border-left: 1px solid var(--line);
    }

    /* Product */
    .product-section {
      padding-block: clamp(4.5rem, 9vw, 7rem);
      background: var(--paper);
    }

    .product-layout {
      display: grid;
      grid-template-columns: 1fr 0.9fr;
      align-items: center;
      gap: clamp(2.5rem, 7vw, 6rem);
    }

    .product-image-wrap {
      position: relative;
      min-height: 440px;
      overflow: hidden;
      background: var(--cream);
    }

    .product-image-wrap img {
      width: 100%;
      height: 100%;
      min-height: 440px;
      object-fit: cover;
    }

    .product-image-label {
      position: absolute;
      right: 1.25rem;
      bottom: 1.25rem;
      padding: 0.65rem 0.85rem;
      background: var(--paper);
      color: var(--forest);
      font-size: 0.78rem;
      font-weight: 700;
      letter-spacing: 0.08em;
      text-transform: uppercase;
    }

    .product-copy .section-title {
      margin-bottom: 1.2rem;
    }

    .product-copy > p:not(.eyebrow) {
      color: var(--muted);
    }

    .product-points {
      display: grid;
      gap: 0.8rem;
      margin: 1.5rem 0 2rem;
      padding: 0;
      list-style: none;
    }

    .product-points li {
      display: flex;
      align-items: baseline;
      gap: 0.75rem;
    }

    .product-points li::before {
      color: var(--leaf);
      content: "—";
      font-weight: 700;
    }

    .text-link {
      color: var(--forest);
      font-weight: 700;
      text-underline-offset: 0.25em;
    }

    /* Story */
    .story-section {
      padding-block: clamp(4.5rem, 9vw, 7rem);
      background: var(--cream);
    }

    .story-layout {
      display: grid;
      grid-template-columns: 0.75fr 1.25fr;
      gap: clamp(2rem, 7vw, 6rem);
      align-items: start;
    }

    .story-heading {
      position: sticky;
      top: 7rem;
    }

    .story-copy {
      max-width: 66ch;
      color: #505b51;
    }

    .story-copy p {
      margin: 0 0 1.2rem;
    }

    .story-quote {
      margin: 2rem 0 0;
      padding: 1.2rem 1.5rem;
      border-left: 3px solid var(--gold);
      color: var(--forest);
      font: italic 1.2rem/1.55 var(--serif);
    }

    /* Ingredients and nutrition */
    .details-section {
      padding-block: clamp(4.5rem, 9vw, 7rem);
      background: var(--paper);
    }

    .details-grid {
      display: grid;
      grid-template-columns: 0.8fr 1.2fr;
      gap: 1.5rem;
      align-items: start;
    }

    .detail-card {
      padding: clamp(1.5rem, 4vw, 2.5rem);
      border: 1px solid var(--line);
      background: white;
    }

    .detail-card h3 {
      margin: 0 0 0.75rem;
      color: var(--forest);
      font: 700 1.55rem/1.25 var(--serif);
    }

    .detail-card > p {
      margin: 0;
      color: var(--muted);
    }

    .ingredient-list {
      display: grid;
      gap: 0.9rem;
      margin: 1.5rem 0 0;
      padding: 0;
      list-style: none;
    }

    .ingredient-list li {
      display: flex;
      gap: 0.7rem;
      align-items: center;
    }

    .check {
      display: grid;
      width: 1.4rem;
      height: 1.4rem;
      flex: 0 0 1.4rem;
      place-items: center;
      border-radius: 50%;
      background: #edf2e8;
      color: var(--forest-light);
      font-size: 0.8rem;
      font-weight: 700;
    }

    .nutrition-caption {
      margin: 0.25rem 0 1rem !important;
      font-size: 0.9rem;
    }

    .table-scroll {
      overflow-x: auto;
      border: 1px solid var(--line);
    }

    .nutrition-table {
      width: 100%;
      border-collapse: collapse;
      text-align: left;
      font-size: 0.93rem;
    }

    .nutrition-table th,
    .nutrition-table td {
      padding: 0.72rem 0.9rem;
      border-bottom: 1px solid var(--line);
    }

    .nutrition-table thead th {
      background: var(--cream);
      color: var(--forest);
      font-weight: 700;
    }

    .nutrition-table tbody th {
      font-weight: 400;
    }

    .nutrition-table td {
      white-space: nowrap;
    }

    .nutrition-table tbody tr:last-child th,
    .nutrition-table tbody tr:last-child td {
      border-bottom: 0;
    }

    /* Experience */
    .experience-section {
      padding-block: clamp(4.5rem, 9vw, 7rem);
      background: var(--forest);
      color: white;
    }

    .experience-section .section-title {
      color: white;
    }

    .experience-section .eyebrow {
      color: #d9c28f;
    }

    .experience-section .section-intro {
      color: rgba(255, 255, 255, 0.76);
    }

    .experience-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 1rem;
    }

    .experience-card {
      padding: clamp(1.5rem, 4vw, 2.25rem);
      border: 1px solid rgba(255, 255, 255, 0.18);
      background: rgba(255, 255, 255, 0.06);
    }

    .experience-card span {
      color: #d9c28f;
      font-size: 0.78rem;
      font-weight: 700;
      letter-spacing: 0.12em;
    }

    .experience-card h3 {
      margin: 0.8rem 0 0.5rem;
      font: 700 1.45rem/1.25 var(--serif);
    }

    .experience-card p {
      margin: 0;
      color: rgba(255, 255, 255, 0.78);
    }

    /* FAQs */
    .support-section {
      padding-block: clamp(4.5rem, 9vw, 7rem);
      background: var(--cream);
    }

    .support-grid {
      display: grid;
      grid-template-columns: 0.75fr 1.25fr;
      gap: clamp(2rem, 6vw, 5rem);
      align-items: start;
    }

    .contact-panel {
      padding: 1.75rem;
      background: var(--paper);
    }

    .contact-panel h3,
    .faq-panel h3 {
      margin: 0 0 1rem;
      color: var(--forest);
      font: 700 1.5rem/1.25 var(--serif);
    }

    .contact-panel p {
      color: var(--muted);
    }

    .contact-link {
      display: block;
      margin-top: 1rem;
      color: var(--forest);
      font-weight: 700;
      overflow-wrap: anywhere;
      text-underline-offset: 0.2em;
    }

    .faq-item {
      border-bottom: 1px solid #dcd9ce;
    }

    .faq-item summary {
      padding: 1rem 2rem 1rem 0;
      color: var(--forest);
      cursor: pointer;
      font-weight: 700;
      list-style: none;
    }

    .faq-item summary::-webkit-details-marker {
      display: none;
    }

    .faq-item summary::after {
      float: right;
      margin-right: -1.6rem;
      color: var(--leaf);
      content: "+";
      font-size: 1.25rem;
    }

    .faq-item[open] summary::after {
      content: "−";
    }

    .faq-item p {
      margin: 0;
      padding: 0 0 1.1rem;
      color: var(--muted);
    }

    /* Footer */
    .site-footer {
      padding-block: 3.5rem 1.25rem;
      background: #102c1d;
      color: white;
    }

    .footer-grid {
      display: grid;
      grid-template-columns: 1.3fr 0.7fr 1fr;
      gap: 3rem;
      padding-bottom: 2.5rem;
    }

    .footer-brand {
      margin: 0 0 0.8rem;
      font: 700 1.5rem/1.2 var(--serif);
    }

    .footer-grid h3 {
      margin: 0 0 1rem;
      color: #d9c28f;
      font-size: 0.82rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
    }

    .footer-grid p {
      max-width: 340px;
      margin: 0;
      color: rgba(255, 255, 255, 0.72);
    }

    .footer-links {
      display: grid;
      gap: 0.6rem;
      margin: 0;
      padding: 0;
      list-style: none;
    }

    .footer-grid a {
      color: rgba(255, 255, 255, 0.82);
      text-decoration: none;
      text-underline-offset: 0.2em;
    }

    .footer-grid a:hover {
      color: #d9c28f;
      text-decoration: underline;
    }

    .footer-bottom {
      padding-top: 1.2rem;
      border-top: 1px solid rgba(255, 255, 255, 0.16);
      color: rgba(255, 255, 255, 0.65);
      font-size: 0.85rem;
      text-align: center;
    }

    .footer-bottom p {
      margin: 0;
    }

    @media (max-width: 800px) {
      .main-nav {
        gap: 0.85rem;
      }

      .main-nav a {
        font-size: 0.8rem;
      }

      .product-layout,
      .story-layout,
      .details-grid,
      .support-grid {
        grid-template-columns: 1fr;
      }

      .product-image-wrap,
      .product-image-wrap img {
        min-height: 360px;
      }

      .story-heading {
        position: static;
      }

      .footer-grid {
        grid-template-columns: 1fr 1fr;
      }

      .footer-grid section:first-child {
        grid-column: 1 / -1;
      }
    }

    @media (max-width: 600px) {
      html {
        scroll-padding-top: 1rem;
      }

      .container {
        width: min(var(--content), calc(100% - 2rem));
      }

      .header-inner {
        min-height: auto;
        align-items: flex-start;
        flex-direction: column;
        gap: 0.75rem;
        padding-block: 0.85rem;
      }

      .main-nav {
        width: 100%;
        justify-content: space-between;
        gap: 0.5rem;
        overflow-x: auto;
        padding-bottom: 0.1rem;
      }

      .main-nav a {
        white-space: nowrap;
      }

      .hero {
        min-height: 76svh;
        background-position: 58% center;
      }

      .hero-content {
        padding-block: 4.5rem;
      }

      .promise-inner {
        grid-template-columns: 1fr;
        padding-block: 0.5rem;
      }

      .promise-item {
        padding: 0.7rem 0;
      }

      .promise-item + .promise-item {
        border-top: 1px solid var(--line);
        border-left: 0;
      }

      .product-image-wrap,
      .product-image-wrap img {
        min-height: 300px;
      }

      .experience-grid,
      .footer-grid {
        grid-template-columns: 1fr;
      }

      .footer-grid section:first-child {
        grid-column: auto;
      }
    }

    @media (prefers-reduced-motion: reduce) {
      html {
        scroll-behavior: auto;
      }

      *,
      *::before,
      *::after {
        transition-duration: 0.01ms !important;
      }
    }
  </style>
</head>

<body>
  <header class="site-header">
    <div class="container header-inner">
      <a class="brand" href="#home" aria-label="Himalayan Bites home">
        <span class="brand-mark" aria-hidden="true">HB</span>
        <span>Himalayan Bites</span>
      </a>

      <nav class="main-nav" aria-label="Main navigation">
        <a href="#story">Our Story</a>
        <a href="#ingredients">Ingredients</a>
        <a href="#experience">Our Promise</a>
        <a href="#contact">Contact</a>
        <a class="nav-cta" href="#product">Discover Ghugute</a>
      </nav>
    </div>
  </header>

  <main>
    <section class="hero" id="home" aria-labelledby="hero-title">
      <div class="container">
        <div class="hero-content">
          <p class="eyebrow">A taste of Uttarakhand</p>
          <h1 id="hero-title">Tradition, made to be shared.</h1>
          <p class="hero-copy">
            Meet Ghugute: a much-loved Himalayan sweet, inspired by the warmth
            of home and the traditions of the mountains.
          </p>
          <div class="hero-actions">
            <a class="button" href="#product">Discover Ghugute <span aria-hidden="true">→</span></a>
            <a class="button button--light" href="#story">Our story</a>
          </div>
          <p class="hero-note">Har Bite Mein Pahadon Ki Shakti</p>
        </div>
      </div>
    </section>

    <div class="promise-strip" aria-label="Product highlights">
      <div class="container promise-inner">
        <div class="promise-item">Inspired by Uttarakhand</div>
        <div class="promise-item">Whole wheat &amp; jaggery</div>
        <div class="promise-item">A tradition worth sharing</div>
      </div>
    </div>

    <section class="product-section" id="product" aria-labelledby="product-title">
      <div class="container product-layout">
        <div class="product-image-wrap">
          <img src="ghugute-product.jpg" alt="Ghugute, traditional Uttarakhand treats">
          <span class="product-image-label">A little taste of home</span>
        </div>

        <div class="product-copy">
          <p class="eyebrow">Meet the mountain crunch</p>
          <h2 class="section-title" id="product-title">A festive favourite, made for everyday moments.</h2>
          <p>
            Ghugute brings together a beloved Uttarakhand tradition and the
            simple pleasure of sharing something delicious. Enjoy it with tea,
            offer it to guests, or make it part of your own family ritual.
          </p>

          <ul class="product-points">
            <li>Made with whole wheat and jaggery</li>
            <li>Inspired by the shapes and stories of Ghughutia</li>
            <li>Thoughtfully packed for gifting and sharing</li>
          </ul>

          <a class="text-link" href="#ingredients">Explore ingredients and nutrition <span aria-hidden="true">→</span></a>
        </div>
      </div>
    </section>

    <section class="story-section" id="story" aria-labelledby="story-title">
      <div class="container story-layout">
        <header class="story-heading">
          <p class="eyebrow">Rooted in tradition</p>
          <h2 class="section-title" id="story-title">The story of Ghugute</h2>
        </header>

        <div class="story-copy">
          <p>
            In the hills of Uttarakhand, Makar Sankranti brings the celebration
            of Ghughutia—a festival that welcomes Uttarayan and the sun’s
            northward journey. At its heart is Ghugute, a sweet treat shaped
            and shared across generations.
          </p>
          <p>
            Local legend tells of a clever crow who helped save a young prince.
            In gratitude, the queen prepared delicacies for the crows. Today,
            children carry garlands of Ghugute and offer the first bites to
            the birds, keeping the story and spirit of the festival alive.
          </p>
          <p>
            Families make Ghugute by kneading wheat flour with jaggery and
            shaping the dough into forms such as flowers, swords, and damarus.
            Once fried until golden, the treats become part of a celebration
            that brings food, family, and folklore together.
          </p>
          <blockquote class="story-quote">
            Some traditions are sweetest when they’re passed around.
          </blockquote>
        </div>
      </div>
    </section>

    <section class="details-section" id="ingredients" aria-labelledby="ingredients-title">
      <div class="container">
        <header class="section-header">
          <p class="eyebrow">Know what’s inside</p>
          <h2 class="section-title" id="ingredients-title">Simple ingredients. Clear information.</h2>
          <p class="section-intro">
            Made with whole wheat and jaggery. Please check the product
            packaging for the latest ingredient and allergen details.
          </p>
        </header>

        <div class="details-grid">
          <article class="detail-card">
            <h3>Our ingredients</h3>
            <p>Inspired by the traditional Ghugute recipe and its familiar flavours.</p>
            <ul class="ingredient-list">
              <li><span class="check" aria-hidden="true">✓</span> Whole wheat</li>
              <li><span class="check" aria-hidden="true">✓</span> Jaggery</li>
              <li><span class="check" aria-hidden="true">✓</span> Made for sharing</li>
            </ul>
          </article>

          <article class="detail-card">
            <h3>Nutrition information</h3>
            <p class="nutrition-caption">Approximate values per 100g</p>
            <div class="table-scroll" tabindex="0" aria-label="Scrollable nutrition information">
              <table class="nutrition-table">
                <caption class="visually-hidden">Approximate nutrition values per 100 grams</caption>
                <thead>
                  <tr>
                    <th scope="col">Parameter</th>
                    <th scope="col">Per 100g</th>
                  </tr>
                </thead>
                <tbody>
                  <tr><th scope="row">Energy</th><td>430–460 kcal</td></tr>
                  <tr><th scope="row">Protein</th><td>6–8g</td></tr>
                  <tr><th scope="row">Total Fat</th><td>12–16g</td></tr>
                  <tr><th scope="row">Carbohydrates</th><td>70–75g</td></tr>
                  <tr><th scope="row">Total Sugars</th><td>30–35g</td></tr>
                  <tr><th scope="row">Added Sugars (Jaggery)</th><td>28–32g</td></tr>
                  <tr><th scope="row">Dietary Fiber</th><td>4–6g</td></tr>
                  <tr><th scope="row">Iron</th><td>2–4mg</td></tr>
                </tbody>
              </table>
            </div>
          </article>
        </div>
      </div>
    </section>

    <section class="experience-section" id="experience" aria-labelledby="experience-title">
      <div class="container">
        <header class="section-header">
          <p class="eyebrow">More than a snack</p>
          <h2 class="section-title" id="experience-title">A little piece of the mountains.</h2>
          <p class="section-intro">
            From the first look inside the package to the last bite, every
            detail is an invitation to share a Himalayan tradition.
          </p>
        </header>

        <div class="experience-grid">
          <article class="experience-card">
            <span>01 / THE UNBOXING</span>
            <h3>A story in every package</h3>
            <p>
              A traditional story card brings the meaning behind Ghugute to
              your table and gives you something lovely to share.
            </p>
          </article>

          <article class="experience-card">
            <span>02 / THE PROMISE</span>
            <h3>Made with care</h3>
            <p>
              We focus on familiar ingredients and thoughtful preparation.
              Check each pack for its full ingredient and allergen information.
            </p>
          </article>
        </div>
      </div>
    </section>

    <section class="support-section" id="contact" aria-labelledby="support-title">
      <div class="container">
        <header class="section-header">
          <p class="eyebrow">Here to help</p>
          <h2 class="section-title" id="support-title">Questions? Let’s talk.</h2>
          <p class="section-intro">Our customer care team is happy to help with your questions.</p>
        </header>

        <div class="support-grid">
          <section class="contact-panel" aria-labelledby="contact-title">
            <h3 id="contact-title">Get in touch</h3>
            <p>For product and order enquiries, send us an email.</p>
            <a class="contact-link" href="mailto:support@himalayanbites.in">
              support@himalayanbites.in
            </a>
          </section>

          <section class="faq-panel" aria-labelledby="faq-title">
            <h3 id="faq-title">Frequently asked questions</h3>

            <details class="faq-item">
              <summary>Are the ingredients organic?</summary>
              <p>
                Please refer to the current product packaging for verified
                sourcing and certification information.
              </p>
            </details>

            <details class="faq-item">
              <summary>Do you use artificial preservatives?</summary>
              <p>
                Please check the ingredients list on your pack for the most
                current product information.
              </p>
            </details>

            <details class="faq-item">
              <summary>How should I store Ghugute?</summary>
              <p>
                Store in a cool, dry place away from direct sunlight. Reseal
                the pouch after opening and follow any storage guidance on
                the packaging.
              </p>
            </details>
          </section>
        </div>
      </div>
    </section>
  </main>

  <footer class="site-footer">
    <div class="container">
      <div class="footer-grid">
        <section>
          <h2 class="footer-brand">Himalayan Bites</h2>
          <p>
            Bringing the taste and traditions of Uttarakhand to your home.
            Har Bite Mein Pahadon Ki Shakti.
          </p>
        </section>

        <nav aria-label="Footer navigation">
          <h3>Explore</h3>
          <ul class="footer-links">
            <li><a href="#story">Our story</a></li>
            <li><a href="#product">Ghugute</a></li>
            <li><a href="#ingredients">Ingredients</a></li>
            <li><a href="#contact">Contact</a></li>
          </ul>
        </nav>

        <section>
          <h3>Say hello</h3>
          <p><a href="mailto:support@himalayanbites.in">support@himalayanbites.in</a></p>
        </section>
      </div>

      <div class="footer-bottom">
        <p>&copy; 2026 Himalayan Bites. All rights reserved.</p>
      </div>
    </div>
  </footer>
</body>
</html>
