---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

[Відповідальність за незаконний перетин кордону під час мобілізації](https://telegra.ph/Vidpovidalnist-za-nezakonnij-peretin-kordonu-pid-chas-mobilizacii-04-03)
[Перелік документів, які є підставою для перетинання державного кордону]({{ site.baseurl }}/files/perelic_doc.pdf)


{%- assign default_paths = site.pages | map: "path" -%}
{%- assign page_paths = site.header_pages | default: default_paths -%}
{%- assign titles_size = site.pages | map: 'title' | join: '' | size -%}
<nav>
  <ul>
    {%- for path in page_paths -%}
      {%- assign my_page = site.pages | where: "path", path | first -%}
      {%- if my_page.title -%}
      <li><a class="page-link" href="{{ my_page.url | relative_url }}">{{ my_page.title | escape }}</a></li>
      {%- endif -%}
    {%- endfor -%}
  </ul>
<nav>

