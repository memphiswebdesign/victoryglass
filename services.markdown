---
layout: default
title: Victory Glass Services
subtitle: Page title will be provided here
permalink: /services
---

<div id="services" class="plus-tile-tx pb-3">
	<div class="container thiner pt-2 pb-5 px-3 px-sm-1 center">
		<pre>Veteran Owned & Operated</pre>
		<h1 class="mt-0">Servicing the Desoto County and Greater Memphis areas!</h1>
		<p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.</p>
	</div>
	{% for service in site.service %}
	<div class="service-item container thin">
		<div class="flex fx-apart fx-wrap pt-0">
			<div class="service-info fx-item-2 fx-item-sm-1">
				<h2>{{ service.title }}</h2>
				<p class="pb-1">{{ service.meta | truncate: 260 }}</p>
				<a href="{{ service.url }}" class="btn">Learn more</a>
			</div>
			<div class="service-img fx-item-2 fx-item-sm-1">
				<div class="padding-none">
					<a href="{{ service.url }}">
						<img src="{{ service.img }}" alt="{{ service.title }}" />
					</a>
				</div>
			</div>
		</div>
	</div>
	{% endfor %}
</div>
