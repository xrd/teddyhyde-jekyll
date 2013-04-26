---
layout: page
---
{% include JB/setup %}

<div class="hero-unit">

<h1> {{ site.title }} </h1>

{{ site.tagline }}

</div>

<div class="container-fluid">
<div class="row-fluid">
<div class="span12">

<h3>Latest Posts</h3>

{% for post in site.posts | limit:10 %}
<a href="{{ BASE_PATH }}{{ post.url }}"><h2> {{ post.title }} </h2></a>
{{ post.content | strip_html | truncatewords: 40 }}
<br/>
<em>Posted on {{ post.date | date_to_string }}</em>
<br/>
{% endfor %}
<a href="/archive.html">See all the archives</a>

</div>
</div>
</div>



