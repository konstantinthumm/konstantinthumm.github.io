---
layout: single
title: Kontakt
permalink: /kontakt/
author_profile: true
classes: wide
---

<p>Sie erreichen mich vorzugsweise über LinkedIn oder per E-Mail.</p>

<div style="display:flex;gap:.75rem;flex-wrap:wrap;align-items:center;margin:1rem 0;">
  {%- assign li = site.author.links | where: "label", "LinkedIn" | first -%}
  {%- if li and li.url -%}
    <a class="btn btn--primary" href="{{ li.url }}" target="_blank" rel="me noopener">LinkedIn</a>
  {%- else -%}
    <!-- Fallback: Bitte ggf. Ihre LinkedIn-URL einsetzen -->
    <a class="btn btn--primary" href="https://www.linkedin.com/" target="_blank" rel="noopener">LinkedIn</a>
  {%- endif -%}

  <a id="mail-link" class="btn" href="#" rel="nofollow">E-Mail anzeigen</a>
  <button id="copy-mail" class="btn" type="button" aria-label="E-Mail-Adresse kopieren">Adresse kopieren</button>
</div>

<noscript>
  <!-- Fallback ohne JS -->
  <p>kt [at] konstantinthumm [punkt] de</p>
</noscript>

<script>
(function(){
  // E-Mail wird im Browser zusammengesetzt
  var u1 = "kt";
  var at = String.fromCharCode(64);
  var d1 = "konstantinthumm";
  var d2 = ".de";
  var addr = u1 + at + d1 + d2;

  var link = document.getElementById("mail-link");
  if (link) {
    link.textContent = addr;
    link.href = "mailto:" + addr + "?subject=Kontakt%20über%20Website";
  }

  var btn = document.getElementById("copy-mail");
  if (btn && navigator.clipboard) {
    btn.addEventListener("click", function(){
      navigator.clipboard.writeText(addr).then(function(){
        var old = btn.textContent;
        btn.textContent = "Kopiert ✓";
        setTimeout(function(){ btn.textContent = old; }, 2000);
      });
    });
  }
})();
</script>
