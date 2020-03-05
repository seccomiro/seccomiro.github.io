---
code: web1
---
{% assign subject = site.data.subjects[page.code] %}

# {{ subject.name }}

{% for content in subject.content %}
  - [{{ content.title }}](/files/{{ page.code }}/{{ content.link }})
{% endfor %}