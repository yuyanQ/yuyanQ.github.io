---
permalink: /
title:  "About"
excerpt: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<div class="home-intro">
  <p class="home-intro__lead">I am a <a href="https://www.enseignementsup-recherche.gouv.fr/fr/les-cifre-46510">CIFRE</a> PhD student in Computer Science at <a href="https://www.sorbonne-universite.fr">Sorbonne Université</a>, in collaboration with <a href="https://www.leadbay.ai">LEADBAY</a>.</p>

  <p>My academic journey is rooted in France, where I completed both my Bachelor’s and Master’s degrees at Sorbonne Université, with a focus on the intersection of language and business analysis. Before that, I studied French Literature at Nanjing University of Finance and Economics in China.</p>
</div>

<section class="home-section" aria-labelledby="research-interests">
  <h2 id="research-interests">Research Interests</h2>
  <div class="research-tags" aria-label="Research interests">
    <span class="research-tag">Table Representation Learning</span>
    <span class="research-tag">Knowledge Graphs</span>
    <span class="research-tag">Structured Data</span>
    <span class="research-tag">Semantic Web</span>
  </div>
</section>

<section class="home-section publications-section" id="publications" aria-labelledby="publications-heading">
  <div class="home-section__heading">
    <h2 id="publications-heading">Publications</h2>
    {% if site.author.googlescholar %}
      <a class="home-section__external" href="{{ site.author.googlescholar }}" target="_blank" rel="noopener">Google Scholar <span aria-hidden="true">↗</span></a>
    {% endif %}
  </div>

  <div class="publication-list">
    {% for post in site.publications reversed %}
      <article class="publication-card">
        <div class="publication-card__year">{{ post.date | date: "%Y" }}</div>
        <div class="publication-card__body">
          <h3 class="publication-card__title">{{ post.title }}</h3>

          {% if post.authors %}
            <p class="publication-card__authors">{{ post.authors }}</p>
          {% endif %}

          <p class="publication-card__venue">{{ post.venue_short | default: post.venue }}</p>

          {% if post.paperurl or post.slidesurl %}
            <div class="publication-card__links">
              {% if post.paperurl %}
                <a class="publication-link" href="{{ post.paperurl }}" target="_blank" rel="noopener">Paper <span aria-hidden="true">↗</span></a>
              {% endif %}
              {% if post.slidesurl %}
                <a class="publication-link" href="{{ post.slidesurl | relative_url }}" target="_blank" rel="noopener">Slides <span aria-hidden="true">↗</span></a>
              {% endif %}
            </div>
          {% endif %}
        </div>
      </article>
    {% endfor %}
  </div>
</section>
