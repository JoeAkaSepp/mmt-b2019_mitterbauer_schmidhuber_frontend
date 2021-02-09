---
title: Button
info: These buttons are being used signal interaction.
nav: true
---

# Basic Buttons

A button can contain text or a svg symbol to display it's action. Although any tag can be used for a button, it will only be keyboard focusable if you use a `button` tag or you add the property `tabindex="0"`.

{% include pattern_block.html url='/src/patterns/components/button/default_button.html' %}

{% include pattern_block.html url='/src/patterns/components/button/disabled_button.html' %}

A button can be disabled, pointer events will not occur.

{% include pattern_block.html url='/src/patterns/components/button/block_button.html' %}

A button can be made to fill its parent.

# Advanced Buttons

{% include pattern_block.html url='/src/patterns/components/button/filter_button.html' %}

A filter button is there to filter the data selection.

{% include pattern_block.html url='/src/patterns/components/button/status_buttons.html' %}

A status button shows the current status of a task. This can be "ToDo", "Doing" or "Done".

{% include pattern_block.html url='/src/patterns/components/button/slide_buttons.html' %}

A slide button has the functionality to move a task from one status to another.
