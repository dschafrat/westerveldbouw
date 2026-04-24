---
layout: default
title: Home
permalink: /
---

<section class="hero">
  <div class="container">
    <div class="hero-content">
      <h1>De fundering voor een goede verbouwing</h1>
      <p>Westerveld Bouw realiseert uitbouwen, dakopbouwen en renovaties in Gooi en Eemland. Vakmanschap dat zichtbaar is in het eindresultaat.</p>
      <div class="hero-cta">
        <a href="/portfolio/" class="btn-primary">Bekijk ons werk</a>
        <a href="/contact/" class="btn-secondary">Neem contact op</a>
      </div>
    </div>
  </div>
</section>

<section class="section section-light">
  <div class="container">
    <div class="section-header">
      <h2>Wat wij doen</h2>
      <p>Van ontwerp tot oplevering — wij begeleiden elk project van begin tot eind.</p>
    </div>
    <div class="services-grid">
      <div class="service-card">
        <div class="service-icon">🏗️</div>
        <h3>Uitbouw</h3>
        <p>Meer woonruimte door een professionele aanbouw aan uw woning.</p>
      </div>
      <div class="service-card">
        <div class="service-icon">🏠</div>
        <h3>Dakopbouw</h3>
        <p>Een extra verdieping of slaapkamer door opbouw van uw dak.</p>
      </div>
      <div class="service-card">
        <div class="service-icon">🔨</div>
        <h3>Renovatie</h3>
        <p>Uw woning vernieuwen met oog voor detail en duurzaamheid.</p>
      </div>
      <div class="service-card">
        <div class="service-icon">🛁</div>
        <h3>Badkamer</h3>
        <p>Moderne badkamers op maat, van ontwerp tot afwerking.</p>
      </div>
    </div>
    <div style="text-align:center; margin-top:2.5rem;">
      <a href="/diensten/" class="btn-primary">Alle diensten</a>
    </div>
  </div>
</section>

<section class="section">
  <div class="container">
    <div class="section-header">
      <h2>Recent werk</h2>
      <p>Bekijk een selectie van onze projecten.</p>
    </div>
    <div class="portfolio-grid">
      {% assign recent = site.projects | slice: 0, 3 %}
      {% for project in recent %}
      <div class="portfolio-card">
        <div class="portfolio-card-image">
          {% if project.cover_image %}
          <img src="{{ project.cover_image | relative_url }}" alt="{{ project.title }}">
          {% endif %}
        </div>
        <div class="portfolio-card-body">
          <p class="category">{{ project.category }}</p>
          <h3>{{ project.title }}</h3>
          <p>{{ project.excerpt | strip_html | truncate: 100 }}</p>
          <a href="{{ project.url }}" class="portfolio-card-link">Bekijk project →</a>
        </div>
      </div>
      {% endfor %}
    </div>
    <div style="text-align:center; margin-top:2.5rem;">
      <a href="/portfolio/" class="btn-primary">Alle projecten</a>
    </div>
  </div>
</section>

<section class="cta-banner">
  <div class="container">
    <h2>Klaar om uw woning te transformeren?</h2>
    <p>Vertel ons over uw project en we nemen snel contact met u op.</p>
    <a href="/contact/" class="btn-primary">Gratis adviesgesprek</a>
  </div>
</section>
