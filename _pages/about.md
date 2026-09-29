---
permalink: /
title: "BIOGRAPHY"
author_profile: false
redirect_from:
  - /about/
  - /about.html
---

{% include page-styles.html %}

<style>
  /* Research Interest Badges */
  .interest-pills {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 15px;
    margin-bottom: 30px;
  }

  .pill {
    background-color: var(--port-primary);
    color: #ffffff;
    font-size: 0.85em;
    font-weight: 600;
    padding: 6px 14px;
    border-radius: 4px;
    letter-spacing: 0.03em;
    box-shadow: 0 2px 4px rgba(0,0,0,0.05);
  }

  /* Featured links */
  .featured-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(260px, 1fr));
    gap: 15px;
    margin-top: 20px;
  }

  .featured-card {
    display: flex;
    align-items: flex-start;
    gap: 14px;
    padding: 16px 18px;
    background: var(--port-bg);
    border: 1px solid var(--port-border);
    border-left: 4px solid var(--port-primary);
    border-radius: 6px;
    text-decoration: none !important;
    color: var(--port-text) !important;
    transition: all 0.3s ease;
  }

  a.featured-card:hover {
    transform: translateY(-2px);
    box-shadow: 0 8px 20px rgba(0,0,0,0.05);
  }

  .featured-card i { font-size: 1.3em; color: var(--port-muted); margin-top: 2px; width: 22px; text-align: center; }
  .featured-card .f-title { font-weight: 700; color: var(--port-primary); font-size: 0.92em; line-height: 1.4; }
  .featured-card .f-meta { font-size: 0.8em; color: var(--port-muted); margin-top: 3px; }
  .featured-card.placeholder { border-left-style: dashed; border-left-color: var(--port-muted); opacity: 0.8; }
</style>

<div class="content-text">
  I am a Ph.D. candidate in Political Science at the <strong>University at Albany (SUNY)</strong>, specializing in <strong>data privacy and technology regulation</strong>. My dissertation committee is chaired by <strong>Prof. Patricia Strach</strong>, with <strong>Prof. Luis Luna-Reyes</strong> and <strong>Dr. Virginia Eubanks</strong>. My research examines how U.S. states write and diffuse consumer data privacy laws, the role of model legislation and interest groups in that process, and the policy gaps created by emerging technologies such as AI-enabled hiring.
</div>

<div class="content-text">
  I am an Adjunct Lecturer in UAlbany's Department of Political Science, where I teach courses on public policy, information policy, and politics. I have worked across academia, government, and the nonprofit sector &mdash; as a <strong>Legislative Fellow</strong> in the office of New York State Senator Patricia Fahy, as a Grants and Research Assistant at <strong>SUNY System Administration</strong>, and in policy roles with <strong>Empire State Development</strong> and the <strong>New York State Network for Youth Success</strong>. I currently support a workforce-development initiative for immigrants and refugees at the <strong>Center for Women in Government &amp; Civil Society</strong>.
</div>

<div class="content-text">
  I hold an M.A. in Political Science from UAlbany and a B.A. (Honors) in International Studies from the <strong>University of Kelaniya</strong>, Sri Lanka, where I graduated with First Class Honors as a gold medalist and later served as an Assistant Lecturer. I am committed to advancing equitable and effective technology policies through evidence-based research, advocacy, and public engagement.
</div>

<h2 class="section-title">Research Interests</h2>
<div class="interest-pills">
  <span class="pill">Data Privacy</span>
  <span class="pill">Privacy Regulation</span>
  <span class="pill">Data Governance</span>
  <span class="pill">Emerging Technology Regulation</span>
  <span class="pill">State Policy Diffusion</span>
</div>

<h2 class="section-title">Featured</h2>
{% if site.data.featured and site.data.featured.size > 0 %}
<div class="featured-grid">
  {% for item in site.data.featured %}
  <a class="featured-card" href="{{ item.url }}" target="_blank" rel="noopener">
    <i class="{{ item.icon | default: 'fas fa-link' }}"></i>
    <div>
      <div class="f-title">{{ item.title }}</div>
      <div class="f-meta">{{ item.source }}{% if item.date %} &middot; {{ item.date }}{% endif %}</div>
    </div>
  </a>
  {% endfor %}
</div>
{% else %}
<div class="featured-grid">
  <div class="featured-card placeholder">
    <i class="fas fa-podcast"></i>
    <div>
      <div class="f-title">Features, interviews and media links</div>
      <div class="f-meta">Coming soon</div>
    </div>
  </div>
</div>
{% endif %}
