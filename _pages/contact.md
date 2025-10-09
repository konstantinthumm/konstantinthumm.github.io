---
layout: single
title: Kontakt
permalink: /kontakt/
author_profile: false
---

<h2>Kontakt</h2>
<p>Schreib mir gern eine E-Mail. Die Adresse wird im Browser zusammengesetzt, damit einfache Crawler sie nicht auslesen.</p>

<p id="contact-line" style="display:flex;gap:.5rem;align-items:center;">
  <a id="mail-link" href="#" rel="nofollow">E-Mail anzeigen</a>
  <button id="copy-mail" type="button" aria-label="E-Mail-Adresse kopieren">Adresse kopieren</button>
  <noscript>
    <!-- Fallback ohne JS: Adresse leicht verschleiert -->
    <span>kt [at] konstantinthumm [punkt] de</span>
  </noscript>
</p>

<script>
(function(){
  // Teile getrennt halten (schlicht, aber effektiv)
  var u1 = "kt";                  // lokaler Teil
  var at = String.fromCharCode(64);
  var d1 = "konstantinthumm";
  var d2 = ".de";
  var addr = u1 + at + d1 + d2;

  var link = document.getElementById("mail-link");
  link.textContent = addr;
  link.href = "mailto:" + addr + "?subject=Kontakt%20über%20Website";

  var btn = document.getElementById("copy-mail");
  btn.addEventListener("click", function(){
    navigator.clipboard.writeText(addr).then(function(){
      btn.textContent = "Kopiert ✓";
      setTimeout(function(){ btn.textContent = "Adresse kopieren"; }, 2000);
    });
  });
})();
</script>
