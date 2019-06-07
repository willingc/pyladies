Title: Locations

PyLadies Locations
------------------

::: {#map}
:::

::: {#archive .section}
::: {.social}
{% for chapter in site.chapters %}

::: {.chapter_location meetup-id="{{chapter.meetup_id}}" chapter-name="{{ chapter.name }}"}
::: {.logo-container}
{% if chapter.image %}
![{{chapter.name}}](../assets/images/%7B%7Bchapter.image%7D%7D) {% else
%} ![{{chapter.name}}](../assets/images/pyladies-sq-logo.png) {% endif
%}
:::

### {% if chapter.external\_website %} [{% else %}](%7B%7Bchapter.website%7D%7D) [{% endif %} {{chapter.name}}](/locations/%7B%7Bchapter.website%7D%7D) {#if-chapter.external_website-else-endif-chapter.name .chpts .chapter-name}

### {% if chapter.website %} [](%7B%7Bchapter.website%7D%7D "Website"){.social .icon .link} {% endif %} {% if chapter.email %} [](mailto:%7B%7Bchapter.email%7D%7D "Contact"){.social .icon .vcard} {% endif %} {% if chapter.facebook %} [](https://www.facebook.com/%7B%7Bchapter.facebook%7D%7D "Facebook"){.social .icon .facebook} {% endif %} {% if chapter.github %} [](https://github.com/%7B%7Bchapter.github%7D%7D "GitHub"){.social .icon .github} {% endif %} {% if chapter.twitter %} [](https://twitter.com/%7B%7Bchapter.twitter%7D%7D "Twitter"){.social .icon .twitter} {% endif %} {% if chapter.meetup %} [](http://www.meetup.com/%7B%7Bchapter.meetup%7D%7D/ "Meetup Link"){.social .icon .location} {% endif %} {% if chapter.google\_plus %} [](%7B%7Bchapter.google_plus%7D%7D "Google+"){.social .icon .google-plus} {% endif %} {% if chapter.timepad%} [](https://%7B%7Bchapter.timepad%7D%7D.timepad.ru "Timepad Link"){.social .icon .location} {% endif %} {#if-chapter.website-endif-if-chapter.email-endif-if-chapter.facebook-endif-if-chapter.github-endif-if-chapter.twitter-endif-if-chapter.meetup-endif-if-chapter.google_plus-endif-if-chapter.timepad-endif .chpts .social-icons}
:::

{% endfor %}
:::
:::

{% endblock %}
