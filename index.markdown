---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

{%- assign default_paths = site.pages | map: "path" -%}
{%- assign page_paths = site.header_pages | default: default_paths -%}
{%- assign titles_size = site.pages | map: 'title' | join: '' | size -%}
<nav>
  <ul>
  <li>
    <a class="page-link" target="blank" href="https://telegra.ph/Vidpovidalnist-za-nezakonnij-peretin-kordonu-pid-chas-mobilizacii-04-03">Відповідальність за незаконний перетин кордону під час мобілізації
    </a>
  </li>
  <li>
    <a class="page-link" target="blank" href="https://dpsu.gov.ua/ua/news/uryad-vnis-zmini-do-pravil-peretinannya-derzhavnogo-kordonu-gromadyanami-ukraini/">
      Правил перетинання державного кордону (dpsu.gov.ua)
    </a>
   </li>
   <li>
    <a class="page-link" target="blank" href="{{ site.baseurl }}/files/perelic_doc.pdf">Перелік документів, які є підставою для перетинання державного кордону
    </a>
  </li>
  <li>
    <a class="page-link" target="blank" href="https://ips.ligazakon.net/document/DG220031?an=2">
      Винятки щодо обмеження виїзду за межі України
    </a>
  </li>
    
    

    {%- for path in page_paths -%}
      {%- assign my_page = site.pages | where: "path", path | first -%}
      {%- if my_page.title -%}
      <li><a class="page-link" href="{{ my_page.url | relative_url }}">{{ my_page.title | escape }}</a></li>
      {%- endif -%}
    {%- endfor -%}
  </ul>
</nav>

<h3>Другая информация</h3>

<ul>
  <li>
    <a href="https://zakon.rada.gov.ua/laws/show/z0927-20#Text" target="blank">
      Расшифровка кодов военной специальности
    </a>
  </li>
  <li>
    <a href="https://tetchange.com/?cur_from=CashUSD&cur_to=USDT" target="blank">
      Обмен USD наличные в USDT
    </a>
  </li>
</ul>
