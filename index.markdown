---
layout: default
title: Victory Auto Glass
permalink: /
---

<div class="home-intro plus-tile-tx">
	<div class="container thin"> 
		<div class="flex fx-apart fx-wrap">
			<div class="intro">
				<pre>Trusted & Dependent</pre>
				<h1>Headline here about the business, mission, service that it provides to the community.</h1>
				<p>Lorem Ipsum is simply dummy text of the print and web industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.</p>
			</div>
			<!-- Services Grid -->
			<div class="services-grid">
				<div class="flex fx-apart fx-wrap cards center">
					{% for service in site.service %}
					<div class="fx-item-2">
						<div class="card-item sm">
							<a class="card-link" href="{{ service.url }}" title="service name"></a>
							<div class="card-image">
								<img src="{{ service.img }}" alt="{{ service.title }}" />
							</div>
							<div class="card-meta">
								<h5>{{ service.title }}</h5>
							</div>
						</div>
					</div>
					{% endfor %}
				</div>
			</div>
		</div>
	</div>
</div>

{% include latest-news-widget.html %}
