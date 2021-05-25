---
permalink: "/publications/"
layout: single
# classes: wide
author_profile: true
title: ""
toc: true
toc_label: "Publications"
toc_sticky: true
---



<!-- See also https://github.com/inukshuk/jekyll-scholar to customize your references -->


<!-- Preprints -->
{% capture counter_preprints %}{% bibliography_count --query @unpublished %}{% endcapture %}
{% if counter_preprints != "0" %}

## Preprints & working papers

  {% bibliography --query @unpublished %}
{% endif %}


<!-- Journals->

{% capture counter_article %}{% bibliography_count --query @article %}{% endcapture %}
{% if counter_article != "0" %}

## Journals

  {% bibliography --query @article %}
{% endif %}

<!-- Conferences-->
{% capture counter_inproceedings %}{% bibliography_count --query @inproceedings %}{% endcapture %}
{% if counter_inproceedings != "0" %}

## Conferences

  {% bibliography --query @inproceedings %}
{% endif %}



<!-- Thesis -->
{% capture counter_thesis %}{% bibliography_count --query @thesis %}{% endcapture %}
{% if counter_thesis != "0" %}

## Thesis

  {% bibliography --query @thesis %}
{% endif %}
