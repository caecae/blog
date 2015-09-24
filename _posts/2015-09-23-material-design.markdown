---
layout: post
title:  "Attempting Google Material Design Part I"
date:   2015-09-23
categories: css design 
---

Basic grid:
* Desktop - 12 (> 800px)
* Tablet - 8 (800 - 500)
* Phone - 4 (< 500px)

Class *mdl-grid* is the master container class
{% highlight css %}
<div class="mdl-grid"> 
  <div class="mdl-cell mdl-cell--6-col mdl-cell--2-col-tablet">
    Content 1
  </div>
  <div class="mdl-cell mdl-cell--2-col-phone">
    Content 2
  </div>
  <div class="mdl-cell">
    Content 3
  </div>
</div>
{% endhighlight %}

<div class="mdl-grid"> 
  <div class="mdl-cell mdl-cell--6-col mdl-cell--2-col-tablet">
    Content 1
  </div>
  <div class="mdl-cell mdl-cell--2-col-phone">
    Content 2
  </div>
  <div class="mdl-cell">
    Content 3
  </div>
  <div class="mdl-cell mdl-cell--hide-tablet">
    Non-tablet Content 3
  </div>
</div>

### Utility class (BEM)

* mdl-cell--stretch; stretches the column to fill the parent element, in this case, mdl-grid.
* mdl-cell--top; aligns the column to the top of the parent.
* mdl-cell--bottom; aligns the column to the bottom or the parent.
