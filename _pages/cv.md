---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
cv_pdf: /files/Yuyan_Qian_CV.pdf
# Update this date whenever the PDF is replaced.
cv_updated: 2026-11-16
---

{% assign cv_pdf_url = page.cv_pdf | relative_url %}
{% assign cv_version = page.cv_updated | date: "%Y-%m-%d" %}
{% assign cv_pdf_url = cv_pdf_url | append: "?v=" | append: cv_version %}

<div class="cv-page">
  <div class="cv-toolbar">
    <p class="cv-updated">Last updated: <time datetime="{{ cv_version }}">{{ page.cv_updated | date: "%B %-d, %Y" }}</time></p>
    <div class="cv-actions">
      <a class="btn btn--info" href="{{ cv_pdf_url }}" download="Yuyan_Qian_CV.pdf"><i class="fas fa-download" aria-hidden="true"></i> Download PDF</a>
      <a class="cv-open" href="{{ cv_pdf_url }}" target="_blank" rel="noopener">Open in a new tab <span aria-hidden="true">↗</span></a>
    </div>
  </div>
  <object class="cv-preview" data="{{ cv_pdf_url }}#view=FitH" type="application/pdf" aria-label="Yuyan Qian’s curriculum vitae (PDF)">
    <p>Your browser cannot display this PDF inline. <a href="{{ cv_pdf_url }}" target="_blank" rel="noopener">Open the CV in a new tab</a> or <a href="{{ cv_pdf_url }}" download="Yuyan_Qian_CV.pdf">download the PDF</a>.</p>
  </object>
</div>
