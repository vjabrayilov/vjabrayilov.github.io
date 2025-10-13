---
layout: default
title: Homepage - Yueyang Pan
---

{% if site.data.bio.description %}
<div class="section">
  <div class="bio">
    {{ site.data.bio.description | markdownify }}
  </div>
</div>
{% endif %}

{% if site.data.education %}
## Education
{% include education.html %}
{% endif %}

{% if site.data.experience %}
## Work Experience
{% include experience.html %}
{% endif %}

{% if site.data.publications %}
## Publications
{% include publications.html %}
{% endif %}

{% if site.data.teaching %}
## Teaching
{% include teaching.html %}
{% endif %}

{% if site.data.awards %}
## Awards & Honors
{% include awards.html %}
{% endif %}
