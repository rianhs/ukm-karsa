---
layout: default
title: "Gema Karsa"
---

<h2 style="color: var(--gold); font-family: 'Playfair Display', serif;">Gema Karsa</h2>
<p>Murai (Muara Ragam Inspirasi): Obrolan inspiratif seputar dunia kedokteran hewan.</p>

<hr style="margin: 30px 0; border: 0; border-top: 1px solid #ddd;">

{% for post in site.categories.MURAI %}
  <article style="margin-bottom: 30px; display: flex; align-items: center;">
    <div style="font-size: 2rem; margin-right: 20px; color: var(--gold);"><i class="fas fa-play-circle"></i></div>
    <div>
      <h3 style="margin: 0;"><a href="{{ post.url | relative_url }}" style="text-decoration: none; color: var(--dark);">{{ post.title }}</a></h3>
      <small style="color: #888;">Episode: {{ post.date | date: "%d %B %Y" }}</small>
    </div>
  </article>
{% else %}
  <p style="font-style: italic; color: #888;">Belum ada episode podcast yang diunggah.</p>
{% endfor %}
