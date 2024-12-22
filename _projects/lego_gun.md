---
layout: page
title: Lego Gun
description: It's not what you think. Robot for Lab 10 of intro to robotics.
img: assets/img/lego_gun/Gun_Turret.png
importance: 1
category: finished
related_publications: false
toc:
  sidebar: left
---

### **Finale competition**

Here's a video of the final competition taken by cmu! Sadly we came in second. This was likely because the competition ran way to long as those running it kept on trying to extend it and extend it. This made my team's robot operator have to run for his class presentation, and our backup could not keep up. Good job all around by everyone!

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://youtube.com/embed/9Q7QW16F6Uo" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### **Magazines**

Here's where this idea really shines. Being able to reload in large amounts is perfect. Adding a dovetail and some magnets for consistent aligning, along with a pin to release the fired pieces, and you have a great little mechanism that maximizes success.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/lego_gun/dovetail.jpeg" title="Open state" class="img-fluid rounded z-depth-1" %}
    </div>
     <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/lego_gun/removal_pin.jpeg" title="Open state" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

The first big problem however is that you can't just use gravity to feed. The tilting motion for most targets makes it so that the longer pieces become quite difficult. This possible could have been fixed by having the turret align with the horizontal or slightly less than horizontal, but that would have greatly increased cycling time and dealt a serious blow to the robots consistency.

The better fix was to introduce a spring, just like how toy varients already do. The problem is that these springs are a ompletly custom torsion like spring, and not something that I could buy on such a short time frame. The easy solution however, was to just go to the 3d printer! Printing out a similar "zig zag" shape resulted in mostly fantastic results.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://youtube.com/embed/k8ZnRefyY5M" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/lego_gun/final_spring.jpeg" title="Open state" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

To put them all together, we used a touch of glue, which held plenty well and created these incredible clips!

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/lego_gun/clips.jpeg" title="Open state" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/lego_gun/reload.jpeg" title="Open state" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### **Jamming(accidental double firing)**

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://youtube.com/embed/Mt3dJNKcGzE" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
Damn, did you see that. Absolutley annoying. It double fired. 
The reason why is pretty simple, when the piece is fired, it's still contacting the bunch of colar band, so it pulls it along with it. This results in double firing, or jamming as the forward most peice looses all it's velocity.

The fix is a bit of a wild one, 3d print a rubber band with little teeth. This makes it so that it fires, it actually ends up "kicking" the block forwards, and eliminates the upper rubber bands that were causing dragging. This stops two from firing at once, while also eliminating drag that gave the blocks incosistent firing.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/lego_gun/belt.png" title="Open state" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### **The turret**

Made up of two main parts. One a standard lego piece that used two parts to rotate around itself, another a custom 3d printed "rack" gear.

Using the standard lego piece was almost a must, but it had a small problem. Because it was just precision plastic rubbing against itself, thought had to be put into balancing out the weight of the mechanism. Keeping its center of mass near the pivot point was important. Hollow printing and careful motor placement solved that problem.

The rack was interesting, imperfect within the short timeframe, but it worked quite well with a little pid magic. It wasn't a true rack, and was effectively a section of a 117 tooth 1 modulus gear. A concentric slot was placed to hold the driving gear from the motor into alignment, and another slot was placed behind that went through the motor, creating the pivots that were used for pan and tilt.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/lego_gun/turret2.jpg" title="Open state" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/lego_gun/rack.png" title="Open state" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### **Aligning to shafts**

The first major problem I ran into was keeping the shafts straight. The prints were not coming out perfect, and attempting to apply a press fit onto the shaft did not work great. The solution was to use lightly heat up the plastic before applying it to the shafts. Allowing it to reach it's ductile glass temp before being pressed on and creating a frim hold. Quickly alligning it with a bearing concentric to the shaft further helped.

<div class="row">
     <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://youtube.com/embed/S15akfQVJbc" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://youtube.com/embed/2jo7SLuBs7A" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

### **Flywheel concept**

Inspired by the torpedo launchers, this takes from the other common way to "safely" launch something. Two flywheels spin in opposite directions via gears. The friction imparts a high acceleration, and then fires the object. This time around we were shooting 1x7 lego technic pieces.

This was a weekend and change project right before finals week. Unlike other intro projects, this one had a lovely budget($30). Being the cad monkey I am, I whipped out some designs for a turret, and threw the entire thing onto my little 3d printer to make it come to life. Using tpu and petg for most things, and large rubber bands to handle(initially) the feeding. Two main revision were done to create a working product.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/lego_gun/wheel_mounting.jpeg" title="Open state" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/lego_gun/rubber_feed.jpeg" title="Open state" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
Both halves of the prototype assembly
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
