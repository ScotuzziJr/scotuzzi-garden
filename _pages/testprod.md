---
layout: page
title: Testando em Prod
id: testprod
permalink: /testprod
---

# \<Um podcast de ouvir\>

O **Testando em Prod** é o seu novo podcast de tecnologia. Nele eu alterno entre discussões sobre tecnologia e conversas com pessoas desenvolvedoras. Todos os episódio estão disponíveis no meu canal do <a href="https://www.youtube.com/@marcpy">YouTube</a>. Os episódios também estão disponíveis em formato de texto.

<strong>Últimas atualizações</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
