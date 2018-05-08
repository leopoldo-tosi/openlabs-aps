---
layout: layout1
---
<!-- culturadigitale -->

<p>
<div class="tiles">

{% for post in site.posts %}
    {% if post.path contains 'culturadigitale' %}
    <div class="#">
	<article>
		<b>{{ post.title }}</b>
		{{ post.excerpt}}
		<ul class="actions"> <li><a href="{{site.baseurl}}{{post.url}}" class="button">More</a></li> </ul>
	</article>
    </div>
    {% endif %}
{% endfor %}
</div>
</p>


