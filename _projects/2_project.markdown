---
layout: page
title: GSoC Prep
description: Comminting to Open Source and getting your proposal accepted
img: https://upload.wikimedia.org/wikipedia/commons/thumb/8/85/GSoC-icon.svg/220px-GSoC-icon.svg.png
importance: 2
category: work
---

At first, a huge thanks goes to Virag Umathe. A dear friend of mine who suggested me the Red Hen Organization. 

Red Hen by its description looks quite complicated and unusual for my interests. However, if you go through their projects, yeah, it is the organization you need !!!


I started in late February. However, I never though of getting accepted. Late Februray is pretty bad time to start, because you are late in comparison to several other people, who have already started contributing to the popular organizations. 

By looking at the multimodal theme, I though I could contribute a style transfer tool to them. This way, I would also gain some domain knowlegde or insights into the style transfer literature. 

Red Hen had already provided a Latex template to write the proposal with a few guidelines. So, the main structure of proposal was already provided and I had to just formulate my knowledge as directed by the template. 

Red Hen, however, thought that style transfer is not what they are interested in. But as a substitute, they suggested me if style transfer can be used in anonymizing audio-visual data. 

I guess, Red Hen was quite correct in case of audio. Yes, style change in audio can be a good way for anonymization. Then, I had to just search for image anonymization. Once the image anonymization was done, video anoymization would be a trivial job. 

To my surprise, `there were already some works on image anonymization with a well maintained code base, that too in PyTorch`. Well, this reduced my work to half. 

Then about audio, is style transfer really the solution? It seems not. I found a few blogs that showed how style is not enough, and more sound features are to be manipulated.

When I searched for speech anoymization on YouTube, `it was surprising to find that speech anonymization is quite fun activity among people. They used audacity filters to anonymize their voice. This was again an interesting find.`

Now, yes with some more formalization and exactly understanding the demands from Red Hen, my proposal was ready. 

The whole process required almost 2-3 days of sincere work and 3-4 more days of loose work. 



<!-- Every project has a beautiful feature showcase page.
It's easy to include images in a flexible 3-column grid format.
Make your photos 1/3, 2/3, or full width.

To give your project a background in the portfolio page, just add the img tag to the front matter like so:

    ---
    layout: page
    title: project
    description: a project with a background image
    img: /assets/img/12.jpg
    ---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/1.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/3.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/5.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/5.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal it's glory in the next row of images.


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/6.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/11.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>


The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/" target="_blank">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/6.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/11.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
``` -->
