---
title: "Home"
layout: homelay
permalink: /
---

<h1 class="home-hero">{{ site.name }}</h1>
<p class="home-hero-sub">{{ site.title }}, {{ site.institution }} · <a href="{{ site.lab.url }}">{{ site.lab.name }}</a></p>

How does a stream of sound become language in the brain? I'm a post-doctoral fellow in [Dr. Christian Brodbeck's lab]({{ site.lab.url }}) at McMaster University, where I use MEG recordings and computational models to trace how the human brain turns speech into meaning.

<div class="chip-container" markdown="0">
<a href="{{ '/research' | relative_url }}" class="chip">Language and the brain</a>
<a href="{{ '/research' | relative_url }}" class="chip">Speech and MEG</a>
<a href="{{ '/research' | relative_url }}" class="chip">Language and action</a>
<a href="{{ '/research' | relative_url }}" class="chip">Robotics</a>
<a href="{{ '/research' | relative_url }}" class="chip">Embodied learning</a>
</div>

{% capture selected %}{% bibliography --query @*[selected=true] %}{% endcapture %}
{% if selected contains "pub-entry" %}
## Selected publications

<div class="section-card selected-pubs" markdown="0">
{{ selected }}
<p style="margin: var(--space-4) 0 0;"><a href="{{ '/publications' | relative_url }}">All publications &rarr;</a></p>
</div>
{% endif %}

## About me

I'm fascinated by how minds, biological and artificial, come to understand language. My path here has crossed several fields: from biotechnology and metabolic neuroscience, to cognitive science, to a PhD in cognitive robotics at the Okinawa Institute of Science and Technology. There, I built brain-inspired neural networks that let robots learn words and actions together, and showed how they can combine familiar concepts in new ways ([*Science Robotics*, 2025](https://doi.org/10.1126/scirobotics.adp0751)).

Today I bring that computational lens to the human brain. By modelling how the brain responds, moment by moment, to natural speech, I study how we pick out words and build meaning in real time.

My full publication record is on [Google Scholar]({{ site.links.google_scholar }}).
