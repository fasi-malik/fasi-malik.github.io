---
layout: default
permalink: /urdu/poetry/
title: اردو شاعری
nav: false
urdu: true
---

<div class="post urdu-page" dir="rtl" style="text-align: right;">
  <div class="header-bar" style="text-align: center; direction: rtl;">
    <h1 style="font-family: 'Jameel Noori Nastaleeq', serif; font-size: 3em; color: #b300b3;">
      {{ page.title }}
    </h1>
    <h2 style="font-family: 'Jameel Noori Nastaleeq', serif; font-size: 1.8em;">
      اردو شاعری — احساسات اور الفاظ کی دنیا
    </h2>
  </div>

  {%- assign urdu_poems = site.urdu_poetry | sort: 'date' | reverse -%}

  {%- comment %} FEATURED (only Urdu poems marked featured: true) {%- endcomment -%}
  {%- assign featured_poems = urdu_poems | where: 'featured', true -%}
  {%- if featured_poems.size > 0 -%}
    <br>
    <div class="container featured-posts">
      {%- assign is_even = featured_poems.size | modulo: 2 -%}
      <div class="row row-cols-{% if featured_poems.size <= 2 or is_even == 0 %}2{% else %}3{% endif %}">
        {%- for poem in featured_poems -%}
          <div class="col mb-4">
            <a href="{{ poem.url | relative_url }}">
              <div class="card hoverable" style="direction: rtl; text-align: right;">
                <div class="row g-0">
                  <div class="col-md-12">
                    <div class="card-body">
                      <div class="float-left"><i class="fa-solid fa-star fa-xs"></i></div>
                      <h3 class="card-title" style="font-family: 'Jameel Noori Nastaleeq', serif;">
                        {{ poem.title }}
                      </h3>
                      {% if poem.description %}
                        <p class="card-text" style="font-family: 'Jameel Noori Nastaleeq', serif;">
                          {{ poem.description }}
                        </p>
                      {% endif %}
                      <p class="post-meta">
                        <i class="fa-solid fa-calendar fa-sm"></i> {{ poem.date | date: "%B %Y" }}
                      </p>
                    </div>
                  </div>
                </div>
              </div>
            </a>
          </div>
        {%- endfor -%}
      </div>
    </div>
    <hr>
  {%- endif -%}

  {%- comment %} LIST ALL POEMS {%- endcomment -%}
  <ul class="post-list" style="font-family: 'Jameel Noori Nastaleeq', serif;">
    {%- for poem in urdu_poems -%}
      <li>
        <h3><a class="post-title" href="{{ poem.url | relative_url }}">{{ poem.title }}</a></h3>
        {% if poem.description %}
          <p>{{ poem.description }}</p>
        {% endif %}
        <p class="post-meta">
          <i class="fa-solid fa-calendar fa-sm"></i> {{ poem.date | date: "%B %d, %Y" }}
        </p>
      </li>
    {%- endfor -%}
  </ul>

  {%- if urdu_poems.size == 0 -%}
    <p>ابھی تک کوئی شاعری شامل نہیں کی گئی۔</p>
  {%- endif -%}
</div>
