# HTML/CSS Review

This is a review of your working knowledge of HTML and CSS. Note that this review is designed to help you recall and familiarize yourself with technical concepts.

## Getting Started

* Fork and clone this repository
* Answer the following questions by...
  * Opening this file in Sublime
  * Answering the questions via Markdown. Feel free to refer to this [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* Commit your changes
* Make a pull request for submission

---

## HTML

1.) Create a valid, empty HTML page with the necessary tags.

```html
<!-- Code goes here -->
<!DOCTYPE html>
<html>
<head>
  <title></title>
</head>
<body>

</body>
</html>
```

2.) What are the differences between these tags?

```html
<!-- Tag 1 -->
<img src="images/me.jpg" alt="My profile image">


<!-- Tag 2 -->
<div></div>
```

```
Explain here.
The first tag will display in image with the relative path of 'images/me.jpg'. If nothing is found, the text "My profile image" will appear.

The second tag, the 'div' tag, is a generic block style element which seems to be used for identifying certain places for javascript
```

---

## CSS

1.) Compare and contrast the following ways to add CSS to HTML elements.

```html
<!-- Inline CSS -->
<div style="background-color: red;"></div>


<!-- Internal style sheet -->
<style type="text/css">
  div {
    background-color: red;
  }
</style>

<!-- External style sheet (not shown) -->
<link rel="stylesheet" type="text/css" href="css/style.css">
```

```
Explain here
Inline --
This way to style elements is to be avoided unless absolutely necessary. This way makes changing styles more difficult since each element must be changed individually.

Internal Style Sheet --
This method is better than strict inline styling, but not as good as an external sheet.  This way makes the html page much longer and can be tedious to change styles.

External Style Sheet --
This is the preferred method.  It separates the two sheets and makes it easier to add/subtract styles, and it is easier for others to jump in and read the code.
```

2.) Below are some different CSS selectors. Use CSS comments to describe what each selector will do.

```css
/* this will give a border circle radius of up to half (I think any more is unnecessary), effectively making the border a circle around the div element */
div {
  border-radius: 50%;
}

/*all paragraph children of header classes will have a font size of 18px. */
.header p {
  font-size: 18px;
}

/*all footer classes will be positioned on the very bottom of the page */
.footer {
  position: absolute;
  bottom: 0;
}

/*all elements with splash-image class will have a the specified image as a background image that will take up the entire page */
.splash-image {
  background-image: url("../images/ocean.jpg");
  background-size: cover;
  width: 100%;
}

/*all text in elements with class ninja will turn black when the mouse is hovered over it */
.ninja:hover {
  display: none;
  color: black;
}
```

