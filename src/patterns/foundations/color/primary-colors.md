---
title: Primary Colors
styles: abstracts/_variables.scss
maturity: ready
control: exclude
colors: 
  - name: $color-primary
    hex: '#24A'
  - name: $color-white
    hex: 'white'
  - name: $color-black
    hex: 'black'
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

<p>The primary color (#24A) can be referenced as the theme color. It is used for the branding on the logo, hero image and as background color for the menu. The other primary colors, black and white, are being used for texts (as foreground color) on the different elements.</p>

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