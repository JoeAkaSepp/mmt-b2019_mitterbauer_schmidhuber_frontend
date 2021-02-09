---
title: Background Colors
styles: abstracts/_variables.scss
maturity: ready
control: exclude
colors:
    - name: $color-background
      hex: "#EEE"
    - name: $color-background-tasks
      hex: "#DDD"
    - name: $color-background-button
      hex: "#78A"
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

<p>The background colors are used as the colors for the main background of the "board", the background of the "tasks cards" themselves and the buttons used in the menu and on the various sites.</p>

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
