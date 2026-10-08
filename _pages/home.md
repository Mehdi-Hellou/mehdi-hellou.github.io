---
title: "Home"
layout: homelay
permalink: /
---

<h1 class="home-hero">{{ site.name }}</h1>
<p class="home-hero-sub">Researcher in Robotics and AI &middot; {{ site.title }}, {{ site.institution }}</p>

<div class="chip-container" markdown="0">
<a href="{{ '/research' | relative_url }}" class="chip">Theory of Mind</a>
<a href="{{ '/research' | relative_url }}" class="chip">Social Robotics</a>
<a href="{{ '/research' | relative_url }}" class="chip">Human&ndash;Robot Interaction</a>
<a href="{{ '/research' | relative_url }}" class="chip">Reinforcement Learning</a>
<a href="{{ '/research' | relative_url }}" class="chip">Personalisation</a>
</div>

My research focuses on improving social robot behaviours in real-world, human-centred environments by applying the premises of the **Theory of Mind (ToM)** to enable personalised interactions.
This includes designing and testing computational architectures for ToM that consider each user's differences and needs, tailoring the robot's actions by exploiting Reinforcement Learning techniques such as Inverse Reinforcement Learning.

<div class="callout callout-info" markdown="0">
<div class="callout-title">{% include icon.html name="house" class="callout-icon" %} Currently</div>
<p>Research Fellow at the University of Manchester's Cognitive Robotics Lab (<a href="https://corolab.uk/" target="_blank" rel="noopener">COROLAB</a>), working within the EU's Horizon Europe programme <a href="https://primi-project.eu/" target="_blank" rel="noopener">PRIMI</a>.</p>
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

I was previously an Early-Stage Researcher and PhD student at the University of Manchester, working on the Marie Sk&#322;odowska-Curie Innovative Training Networks project [PERSEO](https://www.perseo.eu/){:target="_blank" rel="noopener"}, under the supervision of [Prof. Angelo Cangelosi](https://research.manchester.ac.uk/en/persons/angelo.cangelosi){:target="_blank" rel="noopener"} and [Dr. Samuele Vinanzi](https://sites.google.com/view/samuele-vinanzi/){:target="_blank" rel="noopener"}.
My passion for robotics led me to complete a Master of Engineering in Robotics from Polytech Sorbonne University, followed by a Master's in Computer Science at Sorbonne University Pierre and Marie Curie.
[More about me &rarr;]({{ '/about' | relative_url }})
