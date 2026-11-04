---
layout: default
title: "Vahab Jabrayilov: ML systems performance, accelerators, and low-latency systems"
---

{% if site.data.bio.description %}
<div class="section">
  <div class="bio">
    {{ site.data.bio.description | markdownify }}
  </div>
</div>
{% endif %}

{% if site.data.experience %}
## Work Experience
{% include experience.html %}
{% endif %}

{% if site.data.publications %}
<h2 id="publications"><span class="selected-word">Selected </span>Publications</h2>
{% include publications.html %}
{% endif %}

{% if site.data.talks %}
## Talks
{% include talks.html %}
{% endif %}

{% if site.data.education %}
## Education
{% include education.html %}
{% endif %}

{% if site.data.awards %}
## Honors
{% include awards.html %}
{% endif %}
