---
permalink: /about/
layout: page
title: About Prof. Nageh Allam
description: A brief introduction of Prof. Nageh Allam and the Energy Materials Laboratory (EML).
header-img: images/about.jpg
comments: false
modified: 2025-11-08
breadcrumbs: true
---
<img src="/images/NAllam.jpg" alt="Professor Nageh Allam" style="display:block; margin:0 auto; max-width:80%;">

Prof. **Nageh Allam** is a Professor of Physics at the American University in Cairo (AUC) and the founder of the **Energy Materials Laboratory (EML)**. His research focuses on the design, synthesis, and characterization of nanostructured materials for solar energy conversion, electrochemical storage, and sustainable technologies.  

He received his PhD in Materials Science and Engineering from Pennsylvania State University, USA, and has held visiting positions at leading international institutions. Prof. Allam has published extensively in peer‑reviewed journals and is recognized internationally for his contributions to nanotechnology and energy materials.

His [current research interests]({{site.url}}/research) include:
- Nanostructured semiconductors for solar energy conversion  
- Electrochemical energy storage systems (batteries and supercapacitors)  
- Photocatalytic materials for solar fuels and hydrogen generation  
- Interface engineering and computational modeling of energy materials  

<div class="position-grid">
  {% for position in site.data.positions %}
  <div class="position-card">
    <div class="position-info">
      <h3>{{ position.title }}</h3>
      <div class="position-details">
        {% if position.roles %}
          {% for role in position.roles %}
            <strong>{{ role.title }} ({{ role.dates }})</strong><br>
          {% endfor %}
        {% endif %}
        {{ position.department }}<br>
        {{ position.address }}<br>
        {{ position.location }}<br>
        {% if position.phone %}Office: {{ position.phone }}<br>{% endif %}
        {% if position.mobile %}Mobile: {{ position.mobile }}<br>{% endif %}
        Email: {{ position.email }}<br>
        {% if position.profiles %}
          Department profile: 
          {% for profile in position.profiles %}
            <a href="{{ profile.url }}">{{ profile.lang }}</a>
            {% unless forloop.last %}/{% endunless %}
          {% endfor %}
        {% endif %}
      </div>
    </div>
  </div>
  {% endfor %}
</div>

<div markdown="0">
    <a href="{{ site.url }}/cv/" class="btn btn-info">View HTML CV</a>
    <a href="{{ site.url }}/downloads/CV.pdf" class="btn btn-success">Download PDF</a>
</div>

## About This Website
-----

This website is the homepage of the **Energy Materials Laboratory (EML)** at AUC. It is designed to showcase our research, publications, people, and activities, while also serving as a resource for students and collaborators.  

Key features include:
* Clean, responsive design optimized for clarity and accessibility.  
* Support for inline and display math equations via [MathJax](https://www.mathjax.org/).  
* Syntax‑highlighted code blocks for computational modeling and teaching materials.  
* Structured pages for **Research**, **People**, **Publications**, and **News**.  
* Atom/RSS feeds for updates and publications.  
* SEO optimization and sitemap generation for discoverability.  

This website adopts features from:
* The HPSTR Jekyll Theme by [Michael Rose](https://github.com/mmistakes)  
* The Clean Blog Theme by [David Miller](https://github.com/davidtmiller/)  
* The [TWiStErRob Blog](http://www.twisterrob.net) Theme by [Róbert Sándor Papp](https://github.com/TWiStErRob/twisterrob.github.io)  
