---
layout: single
title: Kontakt
permalink: /kontakt/
classes: "wide"
author_profile: false
---

<h2>Schreib mir eine Nachricht</h2>

<form action="https://api.staticforms.xyz/submit" method="post" class="contact-form">
  <!-- StaticForms -->
  <input type="hidden" name="accessKey" value="sf_jgja03lml6h36c3h4ac3md1b">
  <input type="hidden" name="redirectTo" value="https://konstantinthumm.de/danke/">

  <!-- Honeypot gegen Spam -->
  <input type="text" name="honeypot" style="display:none">

  <label for="name">Name</label><br>
  <input type="text" id="name" name="name" required><br><br>

  <label for="email">E-Mail</label><br>
  <input type="email" id="email" name="email" required><br><br>

  <label for="message">Nachricht</label><br>
  <textarea id="message" name="message" rows="6" required></textarea><br><br>

  <label style="display:flex;gap:.5rem;align-items:flex-start">
    <input type="checkbox" required>
    <span>Ich stimme zu, dass meine Angaben zur Beantwortung der Anfrage verarbeitet werden. Hinweise in der Datenschutzerklärung.</span>
  </label><br>

  <button type="submit">Nachricht senden</button>
</form>
