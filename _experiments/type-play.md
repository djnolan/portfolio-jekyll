---
layout: project-shell
title: Type Play
---

A weekly typographic experiment—often telling or introspective, sometimes just a doodle. This is an abstract typographic diary influenced by the events of my week. A way for me to brand my site, play with type and have an ongoing, low-stress project for 2017.

<section class="type-list">

{% for cover in site.data.covers %}
	<div class="type-list__item">
		<h2 class="type-list__hed">{{ cover.date | date: '%B %d, %Y' }}</h2>
		<div class="type-list__image">
			{% include covers/{{ cover.slug }}.html %}
		</div>
	</div>

{% endfor %}

</section>