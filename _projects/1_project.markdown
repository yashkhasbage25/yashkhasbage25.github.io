---
layout: page
title: The AAAI-2021 Paper
description: My first acacdmic paper
img: https://wikimedia.org/api/rest_v1/media/math/render/svg/d2b255c49df2a6e084b9196ab71a68872a739ead
importance: 1
category: work
---

Glad to share my paper accepted at AAAI-2021. 

    ---
    Authors: Adepu Ravi Shankar*, Yash Khasbage*, Rahul Vigneswaran, Vineeth N Balasubramanian
    Title: A Deeper Look at the Hessian Eigenspectrum of Deep Neural Networks and its Applications to Regularization
    Link: https://arxiv.org/abs/2012.03801
    Code: https://github.com/yashkhasbage25/HTR
    ---

Here, I will summarize our paper. 

* How to study hessians? 
Hessian eigenvalues are the most hunted quantity. But computing them for deep neural networks in painstaking. Recent papers have used the eigen spectrums of hessians for studying them. What are eigenspectrums? They show the probability of an eigenvalue at location `$\lambda$`. Thus, we get a rough estimate of the location of eigenvalues. The numerical computation method that gives the eigenspectrum, gives only the higher eigenspectrum. The algorithm, called as `Lanczos algorithm` accepts the number of eigenvalues to study and it gives you eigenspectrums involving those many eigenvalues. 


* Earlier papers, discussed the descomposition Hess = H + G. This is technically known as Gauss-Newton decomposition. Earlier papers pointed that Hess and G had almost similar eigenspectrum in some epochs of training. 

* `$Hess$` was also found to have exactly C number of outliers, where C = number of classes in classification. 

* In this paper, we take a entirely new perspective of this observation by studying the model at layers. We bring up layer hessians and try relating them with full-network hessian. From now, I will address hessian of full network as full-hessian. 

* We first observe that each of `$Hess_l$` has almost C outliers and `$G_l$` are similar to `$Hess_l$`. Thus, something that happened for full network, also happened for individual layer. 

* Now, we can ask which layer is most similar to full-hessian. We have the eigenspectrums for comparing. 
Thus, converting the spectrums to probability distribution, we can find the distance between them using KL-divergence or wasserstein distance. 
We found that, middle layers are most similar to full-hessian. 

* Later, observing the lower trace of better generalizing networks, we claimed that less trace implies better generalization. Hence, we penalize the trace of neural networks using the Hutchington's trace computation method. We found that penlizing trace does improve generalization.

* If middle layers are most similar to full network, can penalizing middle layers cause penalizing full network? Trying this, we found that it worked much better in some networks. This motivates the use of layer-specific regularizers for efficient computations. 


<!-- ---
layout: page
title: project
description: a project with a background image
img: /assets/img/12.jpg
--- -->

<!-- <div class="row">
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
