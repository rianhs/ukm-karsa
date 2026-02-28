---
layout: default
title: "Warta Karsa"
---

<h2 style="color: var(--gold); font-family: 'Playfair Display', serif;">Rubrik MACAN (Majalah dan Catatan)</h2>
<p>Kumpulan berita organisasi dan catatan aktual seputar kampus.</p>

<hr>

{% for post in site.categories.MACAN %}
  <article style="margin-bottom: 30px;">
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <small>{{ post.date | date: "%d %B %Y" }}</small>
  </article>
{% endfor %}
