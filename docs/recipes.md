---
title: Photo Gallery
layout: collection
permalink: /photos/
collection: recipes
entries_layout: grid
---

Sample document listing for the collection `_recipes`.


---
layout: default
images:
  - image_path: /images/cakes/my1.jpg
    title: Apple Pie
  - image_path: /images/cakes/my2.jpg
    title: Birthday Cake
---
<ul>
  {% for image in page.images %}
    <li><img src="{{ image.image_path }}" alt="{{ image.title}}"/></li>
  {% endfor %}
</ul>