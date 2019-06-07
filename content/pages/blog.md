{% extends \"site.html\" %} {% block title %}Blog{% endblock %} {% block
content %}

::: {#archive .section}
Blog
====

Blog
----

{% for post in posts %} {% if not \'resources\' in post.category and not
\'codeconduct\' in post.category %}

### [{{ post.title }}](%7B%7B%20get_url(post.url)%20%7D%7D)

{{ post.date }}

{{ post.excerpt }} [Read more
→](%7B%7B%20get_url(post.url)%20%7D%7D){.more-link}

{% endif %} {% endfor %}
:::

{% endblock %}
