---
title: The Curious Case of the Winner's Curse
author: Jonathan Rittmo
date: '2020-03-17'
slug: the-curious-case-of-the-winner-s-curse
categories:
  - research
tags:
  - Monte Carlo
  - Simulation
  - Power
  - Winner's Curse
subtitle: ''
summary: ''
authors: []
lastmod: '2020-03-17T14:48:48Z'
featured: no
output:
  blogdown::html_page:
    dev: 'svg'
image: 
  caption: ''
  focal_point: ''
  preview_only: no
projects: []
---


Key concepts:
  - Power = the probability of finding an effect if the effect is true

Have you ever been at a psychology stats lecture listening to your teacher rambling about "power", talking about its importance for your experiment to yield a significant result but without really explaining the "why" of it all? Well, so I have I. It is usually easy enough to grasp that low power = bad, high power = good - it's name kind of gives it away. And given that significance is the holy grail in psychology most students would want a high probability to obtain it. The advice is often to calculate a sample size based on some previous (or just predicted) effect. However, for a two group experiment with a between group design and expected medium effect (which arguably could be seen as optimistic) we would need 64 participants if we want a probability of 0.8 of detecting the effect. 

For many undergraduate students (and researchers in genereal) this is just not plausible. Yet, a lot of studies and dissertations projects obtain significance anyway. In my undergrad stats course I was told that this is evidence for the great magnitude of the effect, i.e. because the power of a test mainly is influenced by the number of participants and the size of the effect, if one is low in a significant study the other must be high - right? In fact this has been the predominant view by some scholars. Recently I stumbled upon [this document](/pdf/Wuensch.pdf), a handout by Karl Wuensch, a psychology professor at East Carolina University from his statistics courses in which he states:

>...If you were to find a significant effect of the drug with only 25 participants, that would speak to
the large effect of the drug. In this case you should not be hesitant to seek publication of your
research, but you should be somewhat worried about having it reviewed by “ignorant experts.” Such
bozos (and they are to be found everywhere) will argue that your significant results cannot be trusted
because your analysis had little power. It is useless to argue with them, as they are totally lacking in
understanding of the logic of hypothesis testing. If the editor cannot be convinced that the reviewer is
a moron, just resubmit to a different journal and hope to avoid ignorant expert reviewers there. 

Yes, it is true that significance in a small sample would speak to the large effect found, but what Karl Wuensch seems to miss is that it does speak to the large effect *in the sample*. This does not necessarily (and most probably) not to the population of interest. Perhaps one is not interested in generalising findings and solely in describing one's sample - however, I think that most would agree that this is not what the majortiy of psychologists want. 

But why does not the effect we have found in the sample generalise to the population just because we have low power? Well, intuitively, which score on an IMDB film rating would you rather trust, an average of 9/10 given by 5 people or an average of 6/10 given by 100 people? My guess is that most would say the latter - because we put trust in numbers. In science this translates to a phenomenon called the winner's curse. That is the tendency to over estimate the effect size in under powered studies, due to the fact that only the studies that happen to draw a *sample* with a large effect will obtain a significant result. Together with the publication bias (i.e. significant studies gets more published) this can yield a serious inflation of the effect sizes. 

To demonstrate this it is useful to look at how such overestimation will affect a field "in the long run". 



<div class="figure" style="text-align: left">
<img src="/post/curious-case-of/index_files/figure-html/standard-plot-1.svg" alt="Median overestimation with Crawford and Howell (1998) method, 10^6^ simulations for every parameter combination." width="100%" />
<p class="caption">Figure 1: Median overestimation with Crawford and Howell (1998) method, 10^6^ simulations for every parameter combination.</p>
</div>

