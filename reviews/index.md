---
layout: default
title: "reviews"
date: 2016-02-22 17:06:25
---
{% for post in site.categories.reviews %}

<div class="items-wrapper">
	<div class="item">
	    <a href="{{ site.url }}{{ post.url }}" class="post-link">
		<img alt="{{ post.book }}" src="../reviews/{{ post.book-alt }}.png" style="width:200px;height:200px" />
		<p><a href="{{ site.url }}{{ post.url }}">{{ post.title }}<br />
		<br />
		review by {{ post.author }}</p></a>
	</div>
</div><br><br><br><br><br><br><br><br><br><br>
		
{% endfor %}