---
layout: full-width
title: Reviews
---
<br /><br />
<ul class="content-listing">
	{% for post in site.categories.reviews %}   
		<li class="listing">
	          <a href="{{ post.url | prepend: site.baseurl }}"><h3 class="contrast">{{ post.title }}</h3></a>
	          <br><span class="smaller">by {{ post.author }} on {{ post.date | date: "%B %-d, %Y" }}</span>  <br/>
		    	{{ post.content | strip_html | truncatewords:75}}<br>
		    	<a href="{{ post.url }}">Read more...</a><br><br>
	          <br /><center><hr></center><br /><br />
	{% endfor %}
</ul>