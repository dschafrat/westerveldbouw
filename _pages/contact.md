---
layout: page
title: Contact
permalink: /contact/
description: Neem contact op met Westerveld Bouw voor een vrijblijvend adviesgesprek.
---

<div class="contact-grid">
  <div class="contact-form">
    <h2>Stuur een bericht</h2>
    <form name="contact" method="POST" action="/bedankt/" data-netlify="true">
      <div class="form-group">
        <label for="naam">Naam</label>
        <input type="text" id="naam" name="naam" required>
      </div>
      <div class="form-group">
        <label for="email">E-mailadres</label>
        <input type="email" id="email" name="email" required>
      </div>
      <div class="form-group">
        <label for="telefoon">Telefoonnummer</label>
        <input type="tel" id="telefoon" name="telefoon">
      </div>
      <div class="form-group">
        <label for="onderwerp">Onderwerp</label>
        <select id="onderwerp" name="onderwerp">
          <option value="">Kies een onderwerp</option>
          <option>Uitbouw</option>
          <option>Dakopbouw</option>
          <option>Renovatie</option>
          <option>Badkamer</option>
          <option>Schuur naar kantoor</option>
          <option>Veranda</option>
          <option>Rietenkap</option>
          <option>Anders</option>
        </select>
      </div>
      <div class="form-group">
        <label for="bericht">Uw bericht</label>
        <textarea id="bericht" name="bericht" required></textarea>
      </div>
      <button type="submit" class="btn-primary">Verstuur bericht</button>
    </form>
  </div>

  <div class="contact-info">
    <h3>Contactgegevens</h3>
    <p><strong>Westerveld Bouw</strong></p>
    <p>Gooi en Eemland</p>
    <p>📞 Telefoonnummer volgt</p>
    <p>✉️ E-mail volgt</p>

    <h3 style="margin-top:2rem;">Werkgebied</h3>
    <p>Wij zijn actief in Gooi en Eemland, waaronder Eemnes, Laren, Blaricum, Huizen en omliggende gemeenten.</p>

    <h3 style="margin-top:2rem;">Bereikbaarheid</h3>
    <p>Maandag t/m vrijdag: 08:00 – 17:00</p>
  </div>
</div>
