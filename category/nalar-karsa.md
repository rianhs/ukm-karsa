---
layout: default
title: "Nalar Karsa"
---

<h2 style="color: var(--gold); font-family: 'Playfair Display', serif;">Nalar Karsa</h2>
<p>Kuda (Kupasan Data): Ulasan artikel ilmiah, bedah data, dan analisis ilmu veteriner.</p>

<hr style="margin: 30px 0; border: 0; border-top: 1px solid #ddd;">

{% for post in site.categories.KUDA %}
  <article style="margin-bottom: 30px;">
    <h3 style="margin-bottom: 5px;"><a href="{{ post.url | relative_url }}" style="text-decoration: none; color: var(--dark);">{{ post.title }}</a></h3>
    <small style="color: #888;">{{ post.date | date: "%d %B %Y" }} • Oleh {{ post.author }}</small>
  </article>
{% else %}
  <p style="font-style: italic; color: #888;">Belum ada konten di rubrik ini.</p>
{% endfor %}
