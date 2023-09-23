---
layout: distill
title: TrafficBots
description: "TrafficBots: Towards World Models for Autonomous Driving Simulation and Motion Prediction"
date: 2023-08-22
permalink: /trafficbots

authors:
  - name: Zhejun Zhang
    url: "https://www.trace.ethz.ch/team/members/zhejun.html"
    affiliations:
      name: CVL, ETH Zürich
  - name: Alex Liniger
    url: "https://www.linkedin.com/in/alexander-liniger/"
    affiliations:
      name: CVL, ETH Zürich
  - name: Dengxin Dai
    url: "https://www.linkedin.com/in/dengxin-dai-2412725a/"
    affiliations:
      name: CVL, ETH Zürich
  - name: Fisher Yu
    affiliations:
      name: CVL, ETH Zürich
  - name: Luc Van Gool
    url: "https://www.trace.ethz.ch/team/members/luc.html"
    affiliations:
      name: CVL, ETH Zürich <br> PSI, KU Leuven

# Below is an example of injecting additional post-specific styles.
# If you use this post as a template, delete this _styles block.
_styles: >
  .fake-img {
    background: #bbb;
    border: 1px solid rgba(0, 0, 0, 0.1);
    box-shadow: 0 0px 4px rgba(0, 0, 0, 0.1);
    margin-bottom: 12px;
  }
  .fake-img p {
    font-family: monospace;
    color: white;
    text-align: left;
    margin: 12px 0;
    text-align: center;
    font-size: 16px;
  }

toc:
  - name: Abstract
    # if a section has subsections, you can add them as follows:
    # subsections:
    #   - name: Example Child Subsection 1
    #   - name: Example Child Subsection 2
  - name: Overview
  - name: Supplementary Videos
  - name: Citation
  # - name: Layouts
  # - name: Other Typography?

---
<center>
<div class="links">
<a href="https://arxiv.org/abs/2303.04116" class="btn btn-sm z-depth-1" role="button" target="_blank">arXiv</a>
<a href="https://github.com/SysCV/TrafficBots" class="btn btn-sm z-depth-1" role="button" target="_blank">Code</a>
<a href="/assets/pdf/trafficbots_arxiv.pdf" class="btn btn-sm z-depth-1" role="button" target="_blank">PDF</a>
<a href="/assets/pdf/trafficbots_poster.pdf" class="btn btn-sm z-depth-1" role="button" target="_blank">Poster</a>
<a href="/assets/pdf/trafficbots_slides.pdf" class="btn btn-sm z-depth-1" role="button" target="_blank">Slides</a>
</div>
</center>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/trafficbots-banner.jpg" title="trafficbots banner" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

## Abstract

Data-driven simulation has become a favorable way to train and test autonomous driving algorithms. The idea of replacing the actual environment with a learned simulator has also been explored in model-based reinforcement learning in the context of world models. In this work, we show data-driven traffic simulation can be formulated as a world model. We present TrafficBots, a multi-agent policy built upon motion prediction and end-to-end driving, and based on TrafficBots we obtain a world model tailored for the planning module of autonomous vehicles. Existing data-driven traffic simulators are lacking configurability and scalability. To generate configurable behaviors, for each agent we introduce a destination as navigational information, and a time-invariant latent personality that specifies the behavioral style. To improve the scalability, we present a new scheme of positional encoding for angles, allowing all agents to share the same vectorized context and the use of an architecture based on dot-product attention. As a result, we can simulate all traffic participants seen in dense urban scenarios. Experiments on the Waymo open motion dataset show TrafficBots can simulate realistic multi-agent behaviors and achieve good performance on the motion prediction task.

## Overview
<iframe width="720" height="405" src="https://www.youtube.com/embed/bhZuPpUoiak" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Supplementary Videos

<iframe width="720" height="405" src="https://www.youtube.com/embed/2idvJOqbXeo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Citation

{% highlight bibtex %}
@inproceedings{zhang2023trafficbots,
  title = {TrafficBots: Towards World Models for Autonomous Driving Simulation and Motion Prediction},
  booktitle = {International Conference on Robotics and Automation (ICRA)},
  author = {Zhang, Zhejun and Liniger, Alexander and Dai, Dengxin and Yu, Fisher and Van Gool, Luc},
  year = {2023},
}
{% endhighlight %}
