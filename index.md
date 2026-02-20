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
    <div class="hero-meta">
      <span>{{ site.data.profile.title }}</span>
      <span>{{ site.data.profile.location }}</span>
    </div>
  </section>

  <section class="grid">
    <article class="card">
      <h2>About me</h2>
      {% for paragraph in site.data.profile.about %}
      <p>{{ paragraph }}</p>
      {% endfor %}
    </article>

    <article class="card">
      <h2>Experience highlights</h2>
      <ul>
        {% for item in site.data.profile.experience %}
        <li>
          <strong>{{ item.role }}</strong><br />
          {{ item.org }} · {{ item.period }}
        </li>
        {% endfor %}
      </ul>
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
      <h2>Skills</h2>
      <ul>
        {% for skill in site.data.profile.skills %}
        <li>{{ skill }}</li>
        {% endfor %}
      </ul>
    </article>

    <article class="card card-wide">
      <h2>Selected projects</h2>
      <ul>
        {% for project in site.data.profile.projects %}
        <li>
          <strong>{{ project.name }}</strong><br />
          {{ project.description }}
        </li>
        {% endfor %}
      </ul>
    </article>

    <article class="card">
      <h2>Services</h2>
      <ul>
        {% for service in site.data.profile.services %}
        <li>{{ service }}</li>
        {% endfor %}
      </ul>
    </article>

    <article class="card">
      <h2>Ruby + Vercel note</h2>
      <p>
        "The Ruby runtime takes in a Ruby program that defines a singular HTTP
        handler and outputs it as a Vercel Function."
      </p>
      <small>Useful when extending this static portfolio with API routes.</small>
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
    </article>
  </section>
</main>
