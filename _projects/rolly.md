---
layout: page
title: Rolly
description: Rolly Polly Transforming robot
img: assets/img/rolly/v1_closed.jpeg
importance: 1
category: in-progress
related_publications: false
---


### **V1 Assembled**

V1 rolly polly Assembled! Red timing belt pulleys from tpu. Everything else from leftover polycarbonate and pla. Seems great, the use of cheap chinese bearings and the extremly low powered motors(less than 2.5 watts) leaves the object unable to move. That was presumed to happen however, and better to check the fit of it before investing in some more powerful motors. Doing some small tweaks and adjusting cad in the next version. 
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/rolly/v1_open.jpeg" title="Open state" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/rolly/v1_closed.jpeg" title="Closed state" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    V1 assembled!
</div>

### **Manufacturing**

Making parts. Going for speed, most is 3d printed and made on a cnc router. Shaft design and manufacturing was by far the largest slowdown. Initial cad concept was to do multiple keyed shafts to interface with plastic. Switched to a simple d shaft profile for time. Besides the driven shafts on each side, everything else is simple 8mm hollow aluminum tube cut to length and tapped. 
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/rolly/v1_limbs.jpeg" title="Open state" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/rolly/v1_printing.jpeg" title="Closed state" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Manufacturing
</div>




V1 rolly design: Simple cad model to test out ideas. Using random hardware around to test the physical ability for servos to change the shape of the robot while allowing motion to be transferred using a set of long belts.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/rolly/1_cad_open.jpeg" title="Open state" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/rolly/1_cad_closed.jpeg" title="Closed state" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Initial Cad Model
</div>




<!-- 
The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

{% endraw %} -->
