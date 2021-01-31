---
title: Icons
maturity: planned
control: exclude
items:
    - name: Favicon
      path: src/assets/images/icons/favicon/icon.ico
    - name: Tiny
      path: src/assets/images/icons/favicon/icon-16x16.png
    - name: Mini
      path: src/assets/images/icons/favicon/icon-32x32.png
    - name: Small
      path: src/assets/images/icons/favicon/icon-64x64.png
    - name: Regular
      path: src/assets/images/icons/favicon/icon-128x128.png
    - name: Large
      path: src/assets/images/icons/favicon/icon-512x512.png
---

<style>
.set {
  display: flex;
  flex-wrap: wrap;
  margin: 0 -1rem;
  margin-top: 0;
  padding: 0;
  list-style: none;
}
li {
  flex: 1 0 20%;
  margin: 1rem;
}
.image {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100%;
  min-width: 280px;
  height: 300px;
  background-color: whitesmoke;
  border: 1px solid whitesmoke;
  margin-bottom: 1rem;
}
img {
  max-height: 100%;
}
p {
  margin: 0;
}
</style>
<ul class="set">
{% for item in page.items %} 
  <li>
    <div class="image"><img src="{{ site.baseurl }}/{{ item.path }}"/></div>
    <p class="header">{{ item.name }}</p>
    {% if item.path %}<p>{{ item.path }}</p>{% endif %}
  </li>
{% endfor %}
</ul>
