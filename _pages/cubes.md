---
layout: default
permalink: /cubes/
title: cartesian & dedekind cubes | kianc.site
---

## Cartesian and Dedekind cubes

A work in progress on weak orthogonality and the local model structure on cubical presheaves.

[Read the PDF](/papers/cart-ded/main.pdf)

<hr>

## Contents

{% assign toc = site.data.cart_ded_toc %}
{% if toc %}
<ol class="paper-toc">
  {% for section in toc %}
  <li>
    <a href="/papers/cart-ded/{{ section.href }}">
      {%- if section.number %}<span class="toc-num">{{ section.number }}</span> {% endif -%}
      {{ section.title }}
    </a>
    {% if section.subsections %}
    <ul>
      {% for sub in section.subsections %}
      <li>
        <a href="/papers/cart-ded/{{ sub.href }}">
          {%- if sub.number %}<span class="toc-num">{{ sub.number }}</span> {% endif -%}
          {{ sub.title }}
        </a>
      </li>
      {% endfor %}
    </ul>
    {% endif %}
  </li>
  {% endfor %}
</ol>
{% else %}
*The contents are generated from the paper source — run `deploy-html.sh` in the Cart-Ded repo.*
{% endif %}
