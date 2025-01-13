---
layout: page
title: Inicio
id: inicio
permalink: /
---

# \<Olá, mundo\> 🌱

Esse é o meu *digital garden*, um espaço dedicado para registrar minhas ideias e compartilhar minhas experiências. Fique à vontade para explorar.

<strong>Navegue por áreas</strong>

<ul>
    <li><a class="internal-link" href="{{ site.baseurl }}/computacao">Computação</a></li>
</ul>

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
