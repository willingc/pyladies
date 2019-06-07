Title: Resources

Resources we\'ve written
------------------------

{% for post in posts %} {% if \'resources\' in post.category and
\'pyladies\' in post.category %}

### [{{ post.title }}](%7B%7B%20get_url(post.url)%20%7D%7D)

#### {{ post.author }}

{{ post.summary }} [Read more
→](%7B%7B%20get_url(post.url)%20%7D%7D){.more-link}

{% endif %} {% endfor %}

------------------------------------------------------------------------

Other Resources we like
-----------------------

Have a recommendation? [Suggest it!](http://goo.gl/forms/U66Yweodrw) {%
for post in posts %} {% if \'resources\' in post.category and not
\'pyladies\' in post.category %}

### {{ post.title }}

{{ post.content }}

{% endif %} {% endfor %}
:::

{% endblock %}
