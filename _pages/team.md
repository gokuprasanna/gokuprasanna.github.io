---
title: "Team"
layout: page
permalink: /team/
---

# Team


## PI

<div class="section-card">
<div class="pi-card">
<img src="{{ site.photo | prepend: '/images/' | relative_url }}" class="pi-photo" alt="{{ site.name }}" width="160" height="160">
<div>
<h3 class="pi-name">{{ site.name }}</h3>
<p style="font-style: italic; color: var(--text-secondary);">{{ site.title }}, {{ site.institution }}</p>
<div class="pi-links">
{% if site.email %}<a href="mailto:{{ site.email }}" class="icon-link" title="Email" aria-label="Email">{% include icon.html name="envelope" %}</a>{% endif %}
{% if site.links.google_scholar and site.links.google_scholar != "" %}<a href="{{ site.links.google_scholar }}" class="icon-link" title="Google Scholar" aria-label="Google Scholar">{% include icon.html name="google-scholar" %}</a>{% endif %}
{% if site.links.cv and site.links.cv != "" %}<a href="{{ site.links.cv | prepend: '/' | relative_url }}" class="icon-link" title="CV" aria-label="CV">{% include icon.html name="cv" %}</a>{% endif %}
{% if site.links.github and site.links.github != "" %}<a href="{{ site.links.github }}" class="icon-link" title="GitHub" aria-label="GitHub">{% include icon.html name="github" %}</a>{% endif %}
{% if site.links.researchgate and site.links.researchgate != "" %}<a href="{{ site.links.researchgate }}" class="icon-link" title="ResearchGate" aria-label="ResearchGate">{% include icon.html name="researchgate" %}</a>{% endif %}
{% if site.links.orcid and site.links.orcid != "" %}<a href="{{ site.links.orcid }}" class="icon-link" title="ORCID" aria-label="ORCID">{% include icon.html name="orcid" %}</a>{% endif %}
{% if site.links.twitter and site.links.twitter != "" %}<a href="{{ site.links.twitter }}" class="icon-link" title="X" aria-label="X">{% include icon.html name="x-twitter" %}</a>{% endif %}
{% if site.links.linkedin and site.links.linkedin != "" %}<a href="{{ site.links.linkedin }}" class="icon-link" title="LinkedIn" aria-label="LinkedIn">{% include icon.html name="linkedin" %}</a>{% endif %}
</div>
{% if site.data.pi[0].education %}
<ul style="margin-top: var(--space-4);">
{% for education in site.data.pi[0].education %}
<li>{{ education | replace: "-","&#8211;" }}</li>
{% endfor %}
</ul>
{% endif %}
</div>
</div>
</div>

{% if site.data.team_members.size > 0 %}
## Current Students and Postdocs

<div class="team-grid">
{% for member in site.data.team_members %}
<div class="team-card">
<img src="{{ member.photo | prepend: '/images/' | relative_url }}" class="team-photo" alt="{{ member.name }}" width="100" height="100" loading="lazy">
<h3 class="team-name">{{ member.name }}</h3>
<p class="team-info">{{ member.info }}</p>
<div class="team-links">
{% if member.email %}<a href="mailto:{{ member.email }}" class="icon-link" title="Email" aria-label="Email">{% include icon.html name="envelope" %}</a>{% endif %}
{% if member.website %}<a href="{{ member.website }}" class="icon-link" title="Website" aria-label="Website">{% include icon.html name="house" %}</a>{% endif %}
{% if member.scholar %}<a href="{{ member.scholar }}" class="icon-link" title="Google Scholar" aria-label="Google Scholar">{% include icon.html name="google-scholar" %}</a>{% endif %}
{% if member.github %}<a href="{{ member.github }}" class="icon-link" title="GitHub" aria-label="GitHub">{% include icon.html name="github" %}</a>{% endif %}
</div>
</div>
{% endfor %}
</div>
{% endif %}

{% if site.data.alumni.size > 0 %}
## Alumni

<div class="section-card">
<table class="alumni-table">
<thead>
<tr><th>Name</th><th>Duration</th><th>Current Position</th></tr>
</thead>
<tbody>
{% for member in site.data.alumni %}
<tr>
<td>{{ member.name }}</td>
<td>{{ member.duration }}</td>
<td>{{ member.info }}</td>
</tr>
{% endfor %}
</tbody>
</table>
</div>
{% endif %}
