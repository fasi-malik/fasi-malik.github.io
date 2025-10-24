---
layout: default
permalink: /urdu/blogs/
title: اردو بلاگ
nav: false
urdu: true
---

<div class="post urdu-page" dir="rtl" style="text-align: right;">
  <div class="header-bar" style="text-align: center; direction: rtl;">
    <h1 style="font-family: 'Jameel Noori Nastaleeq', serif; font-size: 3em; color: #b300b3;">
      {{ page.title }}
    </h1>
    <h2 style="font-family: 'Jameel Noori Nastaleeq', serif; font-size: 1.8em;">
      اردو بلاگز — تازہ تحریریں اور خیالات
    </h2>
  </div>

  {%- assign urdu_docs = site.urdu_posts | sort: 'date' | reverse -%}

  {%- comment %} FEATURED (only Urdu posts with featured: true) {%- endcomment -%}
  {%- assign featured_posts = urdu_docs | where: 'featured', true -%}
  {%- if featured_posts.size > 0 -%}
    <br>
    <div class="container featured-posts">
      {%- assign is_even = featured_posts.size | modulo: 2 -%}
      <div class="row row-cols-{% if featured_posts.size <= 2 or is_even == 0 %}2{% else %}3{% endif %}">
        {%- for post in featured_posts -%}
          <div class="col mb-4">
            <a href="{{ post.url | relative_url }}">
              <div class="card hoverable" style="direction: rtl; text-align: right;">
                <div class="row g-0">
                  <div class="col-md-12">
                    <div class="card-body">
                      <div class="float-left"><i class="fa-solid fa-thumbtack fa-xs"></i></div>
                      <h3 class="card-title" style="font-family: 'Jameel Noori Nastaleeq', serif;">
                        {{ post.title }}
                      </h3>
                      {% if post.description %}
                        <p class="card-text" style="font-family: 'Jameel Noori Nastaleeq', serif;">
                          {{ post.description }}
                        </p>
                      {% endif %}
                      {% assign read_time = post.content | number_of_words | divided_by: 180 | plus: 1 %}
                      <p class="post-meta">
                        {{ read_time }} منٹ پڑھنے کا وقت &nbsp; &middot; &nbsp;
                        <i class="fa-solid fa-calendar fa-sm"></i> {{ post.date | date: "%B %Y" }}
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

  {%- comment %} LIST ALL URDU POSTS {%- endcomment -%}
  <ul class="post-list" style="font-family: 'Jameel Noori Nastaleeq', serif;">
    {%- for post in urdu_docs -%}
      <li>
        <h3><a class="post-title" href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        {% if post.description %}<p>{{ post.description }}</p>{% endif %}
        <p class="post-meta">
          <i class="fa-solid fa-calendar fa-sm"></i> {{ post.date | date: "%B %d, %Y" }}
          &nbsp; &middot; &nbsp;
          {% assign read_time = post.content | number_of_words | divided_by: 180 | plus: 1 %}
          {{ read_time }} منٹ پڑھنے کا وقت
        </p>
      </li>
    {%- endfor -%}
  </ul>

  {%- if urdu_docs.size == 0 -%}
    <p>ابھی تک کوئی اردو بلاگ پوسٹ نہیں ہے۔</p>
  {%- endif -%}
</div>
