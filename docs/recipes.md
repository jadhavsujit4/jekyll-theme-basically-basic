---
layout: default
images:
  - image_path: /images/cakes/my1.jpg
    title: Apple Pie
  - image_path: /images/cakes/my2.jpg
    title: Birthday Cake
---
<ul style="list-style: none; padding: 0;">
  {% for image in page.images %}
    <li style="display: inline-block; width: 33%;" >
        <img style = "width: 100%;" src="{{ image.image_path }}" alt="{{ image.title}}"/>
    </li>
  {% endfor %}
</ul>

---
title: Photo Gallery
layout: collection
permalink: /photos/
collection: recipes
entries_layout: grid
---

Sample document listing for the collection `_recipes`.


