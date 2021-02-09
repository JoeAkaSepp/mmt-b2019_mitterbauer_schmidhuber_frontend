---
title: Code Conventions
maturity: ready
---

#### Formatting

- In our code we use an indentation of four spaces throughout the whole application.
- For the class names we prefer dashes over camel-casing or underlines.
- We are trying to avoid styling by ID selectors if it's not necessary.
- For a rule with multiple selectors give each selector their own line.
- Between the selectors and the opening brace `{` we put in a space.
- The closing braces `}` we put on a new line.
- Between rule declarations we put a blank line in between.

Good Code-Example:

```scss
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
```

These code conventions are inspired by the [airbnb css / sass styleguide](https://github.com/airbnb/css).

#### File Structure

For the file structure we use the 7-1-pattern but we've removed those folders that weren't used at all. If needed these folders can be added. The full pattern looks like this:

1. base/
1. components/
1. layout/
1. pages/
1. themes/
1. abstracts/
1. vendors/

to

1. main.scss

The 7-1-pattern file structure was inspired by the [sass guidelines](https://sass-guidelin.es/#the-7-1-pattern).

#### Preprocessors

As CSS preprocessor we use [SCSS](https://sass-lang.com/) due to the fact that we dealt with it in our lecture and already are familiar with it.

#### Vendors

For the app to look the same on every browser we use Normalize.css as basic definition for all elements.
