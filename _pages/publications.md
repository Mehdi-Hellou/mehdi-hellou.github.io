---
title: "Publications"
layout: page
permalink: /publications/
---

# Publications

Here are some of my publications. You can find all of them on my <a href="{{ site.links.google_scholar }}" target="_blank" rel="noopener">Google Scholar</a> page.

<input type="text" class="pub-search" id="pubSearch" placeholder="Filter by title, author, or year...">

<div class="section-card" id="pubList">
<h2>Journal Papers</h2>

{% bibliography --query @article %}

<h2>Conference Papers</h2>

{% bibliography --query @inproceedings %}

<h2>Thesis</h2>

{% bibliography --query @phdthesis %}
</div>
