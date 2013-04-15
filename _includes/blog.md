{% for post in site.posts %}
* {{ post.date | date_to_string }} <a href="{{ BASE_PATH }}{{ post.url }}"> {{ post.title }}</a>

{% endfor %}