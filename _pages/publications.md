---
title: "Publications"
layout: page
permalink: /publications/
---

# Publications

For the complete and up-to-date record, visit <a href="{{ site.links.google_scholar }}">Prasanna Vijayaraghavan's Google Scholar profile</a>.

<input type="text" class="pub-search" id="pubSearch" placeholder="Filter by title, author, or year...">

<div class="section-card" id="pubList">
<h2>Preprints</h2>

{% bibliography --query @unpublished %}

<h2>Refereed Journal Articles</h2>

{% bibliography --query @article %}

<h2>Refereed Conference Proceedings</h2>

{% bibliography --query @inproceedings %}
</div>
