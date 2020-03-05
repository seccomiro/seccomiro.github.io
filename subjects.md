---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: null
---
# Hello

## It's me

Hello from the other side.

<ul>
{{site.data.subjects}}
{% assign subjects = (site.data.subjects | sort: 0)  %}
{% for subject_hash in subjects %}
{% assign subject = subject_hash[1] %}
  <li>
    <a href="/subjects/{{ subject.link }}">
      {{ subject.name }}
    </a>
  </li>
{% endfor %}
</ul>