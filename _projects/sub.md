---
layout: page
title: AUV(Submarine)
description: Building Tartan AUV's new submersible.
img: assets/img/sub/lid2.jpg
importance: 1
category: in-progress
related_publications: false
toc:
  sidebar: left
---

### **LID**

Ok, we abandoned the dome lid. It was iconic, it was beautiful, it was going to stop this projects from getting done.
Love it or hate it, we're going with cruder boyancy foam and a flat lid. Plus, the price of aluminum was pretty cheap when we bought this.... so it seemed like a good call.

However, now that we're done with an overengineerd dome, we need to properly remove material from the flat lid. In a fea portions of past engineering classes, I took a crack at generative design. It struggled on the simplistic force loads that those projects offered, but this should be one of the better things for it.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sub/take1.png" title="Fea take 1" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sub/oooh.png" title="Better" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sub/lid_fea.png" title="lid fea" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

I screwed up my units on the first one, but after that quick change it looks pretty good. I left this for a month and then came back for round 2 before starting manufacturing.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://youtube.com/embed/3wDuf9ySoP4" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Quick video, some beautiful machining, and it's alive.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sub/lid2.jpg" class="img-fluid rounded z-depth-1"%}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sub/in-progress.jpeg" title="in-progress.jpeg" class="img-fluid rounded z-depth-1"%}
    </div>
</div>

I need to face the lid, but it fits! A lovely 10 hour machine time on the good old Fadal 4020. I was babying it a little too much and should have given it more on the roughing. The bottom face is done with a ball end mill to allow the small "veins" that were calculated to be machined.

 <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sub/need2face.jpg" title="Need2face" class="img-fluid rounded z-depth-1"%}
</div>

### **HULL**

5 axis cnc from China! A fantastic learning process about the US customs systems, especially when working with a manufacturer who was unfamiliar with the process. Appeared right around new years. Part came out great, with a lovely red anodizing for corrosion resistance.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://youtube.com/embed/p7SZZXa0lEA" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

It took me almost 4 hours to insert all the helicoils, but hopefully the long term reliability will be worth it. The anodizing was not the best in the world. With the relatively shallower pitch from the threads, a majority of the holes required manual re-tapping. It's likely that this was because of the anodizing process, but it also could have been from the thread mill used. In future designs asking the manufacturer to add an increased cut might be a wise choice to prevent that additional time loss.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sub/Hull1.PNG" title="Hull1" class="img-fluid rounded z-depth-1"%}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sub/Hull2.PNG" title="Hull2" class="img-fluid rounded z-depth-1"%}
    </div>
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sub/Hull3.PNG" title="Hull3" class="img-fluid rounded z-depth-1"%}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sub/Hull4.PNG" title="Hull4" class="img-fluid rounded z-depth-1"%}
    </div>
</div>

### **Final Design**

It's official, we've settled on this one. It's boxy as hell, has more mounting that I can count, but it is designed to last. I've been recommended Jiga by an Alumni, and after a long back and forth with one of their sales team, the prices have managed to beat out the competition by over 40%. It will likely come with many difficulties, but it is impressive.

A wild design for the lid, when we start manufacturing it(or don't), I will go into more details. We're going to machine the lead in house to save on costs, and send the hull overseas. It'll eat up a good portion of our budget but should be worth it.

The concept is high electronics, with thrusters mounted around the edges. Only allowing for external cameras. We've struggled with camera optics often,the fact that an inside one's focal length could too easily change, force a portion of the sub to be acrylic, and set the sub's configuration today outweighs the drawbacks of external enclosures. We'll mount modules easily on the bottom with. It seems like enough, and there's a lovely internal hole grid with hopefully plenty of room.

I've designed in upgrade paths with external electronics, plenty penetrator spots(including oversized variant) as well as a partially spec'd external battery system. The team is pretty happy with it, and the green light has been given.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sub/Osprey.png" title="Osprey" class="img-fluid rounded z-depth-1"%}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sub/Osprey_top.png" title="Osprey top" class="img-fluid rounded z-depth-1"%}
    </div>
</div>
