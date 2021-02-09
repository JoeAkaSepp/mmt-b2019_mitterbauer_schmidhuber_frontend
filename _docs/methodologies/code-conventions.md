---
title: Code Conventions
info: Our code conventions define the formatting, file structure, used pre processor and the vendors.
---

{% include pattern_block.html url='/src/patterns/methodologies/code-conventions/code-conventions.html' %}

<h4>Formatting Code Example SCSS</h4>
{% highlight scss %}
.task-content {
    min-width: 0;
    width: 100%;
    background-color: $color-background-tasks;
    font-family: $roboto;

    .duedate {
        font-weight: lighter;
        font-style: italic;
    }

    .top,
    .bottom {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
    }
}
{% endhighlight %}

