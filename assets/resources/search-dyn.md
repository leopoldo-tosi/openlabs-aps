---
layout: layout1
---

<section id="search">
      <!-- TODO: Search section -->

<div class="tiles" style=" columns: 200px 3;">
<form method="get" action="{{site.baseurl}}/assets/resources/search-dyn.html">
	<input type="hidden" name="query" id="search-box" placeholder="Search"  onclick="javascript:doSearch();" />
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
<script src="{{site.baseurl}}/js/lunr.min.js"></script>
<script src="{{site.baseurl}}/js/search-dyn.js"></script>
</div>

</section>

