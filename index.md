---
layout: default
title: Sarah Maia | Senior Developer & Cybersecurity Engineer
---

<main class="page-wrap">
  <section class="hero card">
    <p class="eyebrow">Portfolio</p>
    <h1>{{ site.data.profile.name }}</h1>
    <p class="lead">{{ site.data.profile.intro }}</p>
    <p class="tagline">"{{ site.data.profile.tagline }}"</p>
  </section>

  <section class="grid">
    <article class="card">
      <h2>About me</h2>
      {% for paragraph in site.data.profile.about %}
      <p>{{ paragraph }}</p>
      {% endfor %}
    </article>

    <article class="card">
      <h2>Education</h2>
      <ul>
        {% for item in site.data.profile.education %}
        <li>
          <strong>{{ item.school }}</strong><br />
          {{ item.details }}
        </li>
        {% endfor %}
      </ul>
    </article>

    <article class="card">
      <h2>What I do</h2>
      <ul>
        {% for service in site.data.profile.services %}
        <li>{{ service }}</li>
        {% endfor %}
      </ul>
    </article>

    <article class="card">
      <h2>Contact</h2>
      <p>Let’s build something exceptional.</p>
      <div class="links">
        {% for link in site.data.profile.links %}
        <a href="{{ link.href }}" target="_blank" rel="noreferrer">{{ link.label }}</a>
        {% endfor %}
        <a href="mailto:{{ site.data.profile.email }}">Email</a>
      </div>
      <small>Tip: replace social links with your real profile URLs before publishing.</small>
    </article>
  </section>
</main>
