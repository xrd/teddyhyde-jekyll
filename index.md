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

{% for post in site.posts %}
{{ post.date | date_to_string }} 
<a href="{{ BASE_PATH }}{{ post.url }}"> {{ post.title }}</a>
{% endfor %}

</div>
</div>
</div>



