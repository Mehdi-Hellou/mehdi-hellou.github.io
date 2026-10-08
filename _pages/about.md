---
title: "About"
layout: page
permalink: /about/
---

# About

<div class="section-card">
<div class="pi-card">
<img src="{{ site.photo | prepend: '/images/' | relative_url }}" class="pi-photo" alt="{{ site.name }}" width="160" height="160">
<div>
<h2 class="pi-name">{{ site.name }}</h2>
<p style="font-style: italic; color: var(--text-secondary);">{{ site.title }}, {{ site.institution }}</p>
<div class="pi-links">
{% if site.email %}<a href="mailto:{{ site.email }}" class="icon-link" title="Email" aria-label="Email">{% include icon.html name="envelope" %}</a>{% endif %}
{% if site.links.cv and site.links.cv != "" %}<a href="{{ site.links.cv | prepend: '/' | relative_url }}" class="icon-link" title="CV" aria-label="CV">{% include icon.html name="cv" %}</a>{% endif %}
{% if site.links.google_scholar and site.links.google_scholar != "" %}<a href="{{ site.links.google_scholar }}" class="icon-link" title="Google Scholar" aria-label="Google Scholar">{% include icon.html name="google-scholar" %}</a>{% endif %}
{% if site.links.github and site.links.github != "" %}<a href="{{ site.links.github }}" class="icon-link" title="GitHub" aria-label="GitHub">{% include icon.html name="github" %}</a>{% endif %}
{% if site.links.researchgate and site.links.researchgate != "" %}<a href="{{ site.links.researchgate }}" class="icon-link" title="ResearchGate" aria-label="ResearchGate">{% include icon.html name="researchgate" %}</a>{% endif %}
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

<div class="section-card" markdown="1">

## Hi, my name is Mehdi Hellou

I am a Research Fellow at the University of Manchester's Cognitive Robotics Lab ([COROLAB](https://corolab.uk/){:target="_blank" rel="noopener"}), working within the EU's Horizon Europe programme [PRIMI](https://primi-project.eu/){:target="_blank" rel="noopener"}.
I was previously an Early-Stage Researcher and PhD student at the University of Manchester, working on the Marie Sk&#322;odowska-Curie Innovative Training Networks project [PERSEO](https://www.perseo.eu/){:target="_blank" rel="noopener"}, under the supervision of [Prof. Angelo Cangelosi](https://research.manchester.ac.uk/en/persons/angelo.cangelosi){:target="_blank" rel="noopener"} and [Dr. Samuele Vinanzi](https://sites.google.com/view/samuele-vinanzi/){:target="_blank" rel="noopener"}.

My research focuses on improving social robot behaviours in real-world, human-centred environments by applying the premises of the **Theory of Mind (ToM)** to enable personalised interactions.
This includes designing and testing computational architectures for ToM that consider each user's differences and needs, tailoring the robot's actions by exploiting Reinforcement Learning techniques such as Inverse Reinforcement Learning.

My passion for robotics led me to complete a Master of Engineering in Robotics from Polytech Sorbonne University, followed by a Master's in Computer Science at Sorbonne University Pierre and Marie Curie.

<div class="banner-frame" markdown="0">
<img src="{{ '/images/main_photo.jpeg' | relative_url }}" alt="Mehdi Hellou in University of Manchester graduation robes" width="1200" height="639" loading="lazy">
</div>

</div>

{% if site.data.awards %}
<div class="section-card">
<h3>Awards</h3>
<ul>
{% for award in site.data.awards %}
<li>{{ award.name | replace: "-","&#8211;" }}</li>
{% endfor %}
</ul>
</div>
{% endif %}
