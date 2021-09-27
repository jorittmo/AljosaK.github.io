---
date: "2021-06-27T00:00:00Z"
external_link: ""
image:
  caption: Photo by Will Myers on Unsplash
  
  focal_point: Smart
links:
- icon: github
  icon_pack: fab
  name: Contribute
  url: https://github.com/jorittmo/singcar
slides: example
summary: For statistical comparison of a single case to normative controls.
tags:
- code projects
title: The R package "singcar" 
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""
---

There are many reasons why researchers and clinicians might want to look at
single cases instead of at the average of some group. In certain fields, such as
neuropsychology, this need arises because the pattern of naturally-occurring
brain damage will be unique in each individual case. From a theoretical
perspective, this means that a single patient might be the only available source
of data for a given phenomenon. 
From a practical, clinical perspective,
diagnosis and description of the pattern of cognitive impairment is done at the
individual level. Individual brain-damaged patients are thus often compared to
the healthy population to assess changes in cognitive functioning. If we want to
assess the patient score on some variate Y, for which we do not know the
population parameters, these must be estimated from a sample. Thus, the
single-case of interest is compared to a control sample. There are many other
areas where the application of such methods could also be useful: for example
studies of uncommon human expertise, targeted quality checks in industries with
limited production output, or animal studies where rearing a large experimental
group might be infeasible.

An abnormally low score on
a single variate is in neuropsychology often referred to as a *deficit*, an important concept
for clinical and basic neuropsychology alike. For the latter area another
concept is also considered to be of cardinal importance: the ability to test for
an abnormally large discrepancy between two variates. This is referred to as a
*dissociation*, which is taken to provide evidence for some degree of
functional independence between two cognitive abilities. By charting
dissociations, a cognitive architecture of the mind can be theorized.l

During the last 20 years, a class of related methods have been developed for
case-control comparisons, allowing researchers to estimate abnormality and test
for deficits and dissociations in the single case, while controlling the Type I
error rate. These tests have been developed mainly by John Crawford and Paul
Garthwaite.
John Crawford has provided free software packages to perform these tests, making
them available 
[here](https://homepages.abdn.ac.uk/j.crawford/pages/dept/psychom.htm). However,
these are available only as standalone compiled computer programs for Windows
operating systems. Most of these programs require manual input of summary
statistics, and output a static text file. For thorough documentation one must
consult the original publications.

Our aim is to encourage and simplify usage of these methods by implementing them
in the package singcar for the R environment, bringing them together in a
fully documented package with open source code that works across platforms.
Further advantages of singcar include an API that has more modifiable test
parameters and can operate directly on raw data, reducing the risk of human
error. It is also possible to automate these tests if multiple analyses need to
be run for the purposes of data analysis or simulation studies. 
The development
of Crawford and Garthwaite's methods has been focused around limiting Type I
errors, but to emphasise the importance of limiting Type II errors we also
provide power calculators for each test function. Our hope in doing so is to
increase awareness of power considerations for this methodology as well as to
aid in the planning and design of experiments
[@mcintoshPowerCalculationsSinglecase2020].
