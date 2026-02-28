---
layout: default
title: "Warta Karsa"
---

<h2 style="color: var(--gold); font-family: 'Playfair Display', serif;">Warta Karsa</h2>
<p>Macan (Majalah dan Catatan): Kumpulan berita seputar kampus dan seputar isu kedokteran hewan.</p>

<hr>

{% for post in site.categories["Warta Karsa"] %}
  <article style="margin-bottom: 30px;">
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <small>{{ post.date | date: "%d %B %Y" }}</small>
  </article>
{% endfor %}
