---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

Hi, and welcome to my homepage. Yes, this is yet another "homepage" that is abandoned and left for dead.

Things I intend to put here

- Travel diaries and tales of bold adventures
- TIL; Today I learned.
- Contact information, including my Public GPG key.
- Various stuff I care about
- Podcasts I recommend
- Links to fun stuff on the Internets.

<h2>Blog articles</h2>
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

<h2>Tag categories</h2>
{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
