---
layout: project-shell
title: Type Play
---

Every so often I update my homepage cover art with a new typographic doodle. They’re sometimes meaningful, sometimes not. They're a way to brand my site and play with letters. Here’s the full list.



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