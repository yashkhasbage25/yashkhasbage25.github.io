---
layout: page
title: Unofficial Implementations
description: Unofficial Implementations of Deep Learning Papers
img: https://live.staticflickr.com/5692/30463008682_3c448d3762_b.jpg
importance: 3
category: fun
---

I found out these two papers interesting to implement:

    ---
    layout: page
    Title: The Lottery Ticket Hypothesis: Finding Sparse, Trainable Neural Networks
    Authors: Jonathan Frankle, Michael Carbin
    Link: https://arxiv.org/abs/1803.03635

    My implementation: https://github.com/yashkhasbage25/LTH
    ---

    ---
    layout: page
    Title: Membership Inference Attacks Against Machine Learning Models
    Authors: Reza Shokri, Marco Stronati, Congzheng Song, Vitaly Shmatikov
    Link: https://ieeexplore.ieee.org/document/7958568
    
    My implementation: https://github.com/yashkhasbage25/MemInf
    ---


LTH or the Lottery Ticket hypothesis gained an upsurge in its citations around 2019-2020. I guess the simplicity and great results were crucial in this. It was easy to try in PyTorch.

LTH claims that there exists an extremely sparse network in your deep neural network that achieves almost the same accuracy. They prove it experimentally with their algorithm, which is their contribution. 

Membership inference is the paper from 2015-2016, which boosted differential privacy research in deep learning. I won't be wrong if I call it as a classic paper in its domain. The authors introduce a new concept into the community and provide a simple solution to it. 

I did not focus on getting the exact numbers for both papers. My aim was to understand the implementation details and the extent of robustness in their claims. 