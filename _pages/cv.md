---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<div class="cv-page">

<section class="cv-block">

<h2><i class="fas fa-graduation-cap" aria-hidden="true"></i> Education</h2>

<div class="cv-timeline">

<div class="cv-entry">
<div class="cv-entry-head">
<h3 class="cv-entry-title">PhD in Computer Science</h3>
<span class="cv-entry-date">2025 - Present</span>
</div>
<div class="cv-entry-org">Sorbonne Université &amp; LEADBAY, Paris, France</div>
<ul class="cv-entry-details">
<li>CIFRE PhD Program</li>
<li>Thesis: "Knowledge hypergraphs and neural networks for multimedia and multimodal data: B2B sales application"</li>
<li>Under the supervision of Claude Montacié, María Victoria Eyharabide and Milan Stankovic</li>
</ul>
</div>

<div class="cv-entry">
<div class="cv-entry-head">
<h3 class="cv-entry-title">Master's Degree in Language and Computer Science</h3>
<span class="cv-entry-date">2022 - 2024</span>
</div>
<div class="cv-entry-org">Sorbonne Université, Paris, France</div>
<ul class="cv-entry-details">
<li>Specialized in NLP, LLM, Speech Recognition and Synthesis</li>
<li>Semantic Indexing and Information Retrieval</li>
</ul>
</div>

<div class="cv-entry">
<div class="cv-entry-head">
<h3 class="cv-entry-title">Bachelor's Degree in Linguistics, specialization in computer science</h3>
<span class="cv-entry-date">2021 - 2022</span>
</div>
<div class="cv-entry-org">Sorbonne Université, Paris, France</div>
</div>

<div class="cv-entry">
<div class="cv-entry-head">
<h3 class="cv-entry-title">Bachelor's Degree in French Literature</h3>
<span class="cv-entry-date">2017 - 2021</span>
</div>
<div class="cv-entry-org">Nanjing University of Finance and Economics, Nanjing, China</div>
</div>

</div>
</section>

<section class="cv-block">

<h2><i class="fas fa-briefcase" aria-hidden="true"></i> Experience</h2>

<div class="cv-timeline">

<div class="cv-entry">
<div class="cv-entry-head">
<h3 class="cv-entry-title">CIFRE PhD Student</h3>
<span class="cv-entry-date">June 2025 - Present</span>
</div>
<div class="cv-entry-org">LEADBAY, Paris, France</div>
<ul class="cv-entry-details">
</ul>
</div>

<div class="cv-entry">
<div class="cv-entry-head">
<h3 class="cv-entry-title">Student Researcher</h3>
<span class="cv-entry-date">November 2024 - June 2025</span>
</div>
<div class="cv-entry-org">LEADBAY, Paris, France</div>
<ul class="cv-entry-details">
<li>Research internship focusing on knowledge representation and AI applications</li>
</ul>
</div>

<div class="cv-entry">
<div class="cv-entry-head">
<h3 class="cv-entry-title">Data Scientist Intern</h3>
<span class="cv-entry-date">May 2024 - October 2024</span>
</div>
<div class="cv-entry-org">DARAROCKSTARS, Paris, France</div>
<ul class="cv-entry-details">
<li>Developed AI microservices for recruitment platforms</li>
</ul>
</div>

</div>
</section>

<section class="cv-block">

<h2><i class="fas fa-file-alt" aria-hidden="true"></i> Publications</h2>

<div class="cv-timeline">
{% for post in site.publications reversed %}
<div class="cv-entry">
<div class="cv-entry-head">
<h3 class="cv-entry-title">{{ post.title }}</h3>
<span class="cv-entry-date">{{ post.date | date: "%Y" }}</span>
</div>
<div class="cv-entry-org">{{ post.venue }}</div>
<div class="cv-entry-links">
{% if post.paperurl %}<a class="cv-entry-link" href="{{ post.paperurl }}" target="_blank" rel="noopener">View Paper</a>{% endif %}
{% if post.slidesurl %}<a class="cv-entry-link" href="{{ post.slidesurl | relative_url }}" target="_blank" rel="noopener">Slides</a>{% endif %}
</div>
</div>
{% endfor %}
</div>
</section>

<section class="cv-block">

<h2><i class="fas fa-code" aria-hidden="true"></i> Technical Skills</h2>

<div class="cv-skills">

<div class="cv-skill-group">
<h3>Programming Languages</h3>
<div class="cv-tags">
<span class="cv-tag">Python</span>
<span class="cv-tag">Java</span>
<span class="cv-tag">C++</span>
<span class="cv-tag">SPARQL</span>
<span class="cv-tag">R</span>
</div>
</div>

<div class="cv-skill-group">
<h3>Tools &amp; Frameworks</h3>
<div class="cv-tags">
<span class="cv-tag">Docker</span>
<span class="cv-tag">Elasticsearch</span>
<span class="cv-tag">Postman</span>
<span class="cv-tag">AWS</span>
<span class="cv-tag">Flask</span>
<span class="cv-tag">Neo4j</span>
<span class="cv-tag">TXM</span>
<span class="cv-tag">Unitex</span>
<span class="cv-tag">Praat</span>
<span class="cv-tag">GATE</span>
<span class="cv-tag">Protégé</span>
</div>
</div>

<div class="cv-skill-group">
<h3>Machine Learning</h3>
<div class="cv-tags">
<span class="cv-tag">Scikit-learn</span>
<span class="cv-tag">PyTorch</span>
<span class="cv-tag">TensorFlow</span>
</div>
</div>

<div class="cv-skill-group">
<h3>NLP</h3>
<div class="cv-tags">
<span class="cv-tag">SpaCy</span>
<span class="cv-tag">NLTK</span>
<span class="cv-tag">Gensim</span>
</div>
</div>

<div class="cv-skill-group">
<h3>Data Analysis</h3>
<div class="cv-tags">
<span class="cv-tag">Pandas</span>
<span class="cv-tag">NumPy</span>
</div>
</div>

<div class="cv-skill-group">
<h3>Web Applications</h3>
<div class="cv-tags">
<span class="cv-tag">Streamlit</span>
<span class="cv-tag">Flask</span>
</div>
</div>

</div>
</section>

</div>
