---
layout: splash
permalink: /
hidden: true
header:
  overlay_color: "#5e616c"
  overlay_image: /assets/images/base/intro-01-bw.png
  actions:
    - label: "About"
      url: "/about/"
excerpt: >
  A consortium of academic institutions in Slovenia that integrates the country's research infrastructure focusing on structural biology
feature_row:
  - image_path: /assets/images/base/intro-01-bw.png
    alt: "Instruct-ERIC"
    title: "Instruct-ERIC"
    excerpt: "What [Instrust-ERIC](https://instruct-eric.org/) is about, and what it offers to researchers from member countries."
    url: "instruct-eric"
    btn_class: "btn--primary"
    btn_label: "Learn more"
  - image_path: /assets/images/base/intro-01-bw.png
    alt: "application"
    title: "How to apply"
    excerpt: "How to apply for funded access to the services offered by [Instrust-ERIC](https://instruct-eric.org/)."
    url: "/application/"
    btn_class: "btn--primary"
    btn_label: "Learn more"
  - image_path: /assets/images/base/intro-01-bw.png
    alt: "infrastructure"
    title: "Infrastructure"
    excerpt: "Info on structural biology infrastructure available in Slovenia."
    url: "/infrastructure/"
    btn_class: "btn--primary"
    btn_label: "Learn more"      
---

{% include feature_row %}

# Recent posts

{% if paginator %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

<div class="entries-{{ entries_layout }}">
  {% for post in posts limit:3 %}
    {% include archive-single.html type=entries_layout %}
  {% endfor %}
</div>

[More posts](/instructsi/year-archive/){: .btn .btn--info}