---
title: "Adie Family Papers"
categories:
  - Blog
tags:
  - genealogy
---
A large number of old papers used to live in a big chest in Bellevue, one of the Adie family homes in Voe, Shetland. These papers were donated in 2022 to the [Shetland Archives](https://www.shetlandmuseumandarchives.org.uk/), where they await cataloguing. They contain a great deal of genealogically interesting material, much of which I copied. Rather than that material sitting on my computer, unavailable to the world, I am putting it online, in this repository, in the hope someone will find it useful.

{% for paper in site.family-papers %}

### [{{ paper.title }}]({{ paper.url }})

{{ paper.excerpt }}

{% endfor %}
