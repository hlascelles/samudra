---
layout: kz-page
permalink: "/archive/"
subheadline: subheadline
title: "Blahhh"
teaser: "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua."
header:
    image_fullwidth: "homepage_image.jpg"
---
<div id="blog-index" class="row">
	<div class="small-12 columns t30">
		<dl class="accordion" data-accordion>
			{% assign counter = 1 %}
			{% for post in site.posts limit:1000 %}
			<dd class="accordion-navigation">
			<a href="#panel{{ counter }}"><span class="iconfont"></span> {% if post.date %}{{ post.date | date: "%Y-%m-%d" }}{% endif %} &middot; <strong>{{ post.title }}</strong></a>
				<div id="panel{{ counter }}" class="content">
					{% if post.meta_description %}{{ post.meta_description | strip_html | escape }}{% elsif post.teaser %}{{ post.teaser | strip_html | escape }}{% endif %}
					<a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}" title="Read {{ post.title | escape_once }}"><strong>{{ site.data.language.read_more }}</strong></a><br><br>
				</div>
			</dd>
			{% assign counter=counter | plus:1 %}
			{% endfor %}
		</dl>
	</div><!-- /.small-12.columns -->
</div><!-- /.row -->