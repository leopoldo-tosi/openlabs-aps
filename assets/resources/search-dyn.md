---
layout: layout1
---

<section id="search">
      <!-- TODO: Search section -->

<div class="tiles" style=" columns: 200px 2;">
<form method="get" action="{{site.baseurl}}/assets/resources/search-dyn.html">
	<input type="hidden" name="query" id="search-box" />
</form>
<ul id="search-results"></ul>
<script>
  window.store = {
              {% for post in site.posts %}
                    "{{ post.url | slugify }}": {
        "title": "{{ post.title | xml_escape }}",
        "author": "{{ post.author | xml_escape }}",
        "category": "{{ post.category | xml_escape }}",
        "content": {{ post.content | strip_html | strip_newlines | jsonify }},
        "url": "{{site.baseurl}}{{ post.url | xml_escape }}"
          }
                          {% unless forloop.last %},{% endunless %}
                              {% endfor %}


                                };

</script>
<script src="{{site.baseurl}}/assets/js/lunr.min.js"></script>
<script src="{{site.baseurl}}/assets/js/search-dyn.js"></script>
</div>

</section>

