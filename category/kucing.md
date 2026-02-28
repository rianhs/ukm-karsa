---
layout: default
title: "Arsip KUCING"
---

<h2 style="color: var(--gold); font-family: 'Playfair Display', serif;">Rubrik KUCING (Kumpulan Citra & Infografis)</h2>
<p>Galeri karya visual, poster edukasi, dan infografis kesehatan hewan karya mahasiswa.</p>

<hr style="margin: 30px 0; border: 0; border-top: 1px solid #ddd;">

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px;">
{% for post in site.categories.KUCING %}
  <article style="background: white; padding: 20px; border-radius: 10px; box-shadow: 0 2px 5px rgba(0,0,0,0.05);">
    <h3 style="font-size: 1.1rem;"><a href="{{ post.url | relative_url }}" style="text-decoration: none; color: var(--dark);">{{ post.title }}</a></h3>
    <small style="color: #888;">{{ post.date | date: "%d %B %Y" }}</small>
  </article>
{% else %}
  <p style="font-style: italic; color: #888;">Belum ada konten visual di sini.</p>
{% endfor %}
</div>
