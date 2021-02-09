---
title: Task-Status Colors
styles: abstracts/_variables.scss
maturity: ready
control: exclude
colors:
    - name: $color-status-todo
      hex: "#24A"
    - name: $color-status-doing
      hex: "#29A"
    - name: $color-status-done
      hex: "#2A5"
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
.color {
  width: 100%;
  min-width: 160px;
  height: 80px;
  color: white;
  border: 1px solid whitesmoke;
  margin-bottom: 1rem;
}
p {
  margin: 0;
}
</style>

<p>The task status colors are supposed to show the different status throughout the app. The todo status color aligns with the theme color whereas doing and done are trying to have a certain contrast to each.</p>

<ul class="set">
{% for item in page.colors %} 
  <li>
    <div class="color" style="background:{{ item.hex }}"></div> 
    <p>{{ item.name }}</p>
    {% if item.hex %}<p>{{ item.hex }}</p>{% endif %}
    {% if item.rgb %}<p>{{ item.rgb }}</p>{% endif %}
  </li>
{% endfor %}
</ul>
