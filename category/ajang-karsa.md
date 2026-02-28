---
layout: default
title: "Ajang Karsa"
---

<h2 style="color: var(--gold); font-family: 'Playfair Display', serif;">Ajang Karsa</h2>
<p>Rusa (Ruang Sayembara): Informasi kompetisi ilmiah dan informasi prestasi mahasiswa kedokteran hewan.</p>

<hr style="margin: 30px 0; border: 0; border-top: 1px solid #ddd;">

{% for post in site.categories.RUSA %}
  <article style="margin-bottom: 30px; border-left: 4px solid #e74c3c; padding-left: 20px;">
    <h3 style="margin-bottom: 5px;"><a href="{{ post.url | relative_url }}" style="text-decoration: none; color: var(--dark);">{{ post.title }}</a></h3>
    <small style="color: #888;">Update: {{ post.date | date: "%d %B %Y" }}</small>
  </article>
{% else %}
  <p style="font-style: italic; color: #888;">Belum ada informasi lomba terbaru.</p>
{% endfor %}
