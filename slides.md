Power calculations for mouse research
========================================================
author: Thomas G. Stewart, PhD
date: 13 August 2019
autosize: true
width:1024
height:768
transition: fade
transition-speed: fast

These slides were prepared for the 2019 Vanderbilt Mouse Kidney Injury Workshop [(link)](https://www.mc.vanderbilt.edu/vckd/events/2019/workshop/) on 13 August 2019.

<style>
.reveal h1, .reveal h2, .reveal h3 {
  word-wrap: normal;
  -moz-hyphens: none;
}
.footer {
  color: black; background: none;
  position: fixed; top: 90%;
  text-align:left; width:100%;
}
div.centered {
  position: fixed; 
  top: 25%;
  left:10%;
  text-align:center; 
  width:80%;
  margin:auto;
  border: 0px;
}

.section .reveal .state-background{
background-color:#343777;
}

.reveal pre code{
font-size:1em;
line-height:1.2em;
}

.reveal pre{
margin:0px;
width:99%;
}

.reveal section img{
box-shadow: 0 0 0 0;
}
</style>




Slides
======

<br><br>
These slides are available on my faculty page under **Teaching**
<br><br><br>
<h2>tgstewart.xyz</h2>


The goals of this session are to
========================================================
- provide a big picture overview of power calculations
- explain when power calculations are (and are not) appropriate
- introduce online resources for power calculations
- work through **hands-on** examples of calculating power


The big picture
========================================================

![](data-flow-steps-analysis-expanded-nopublication-01.svg)

The big picture
========================================================
transition: none

![](data-flow-steps-analysis-expanded-nopublication-02.svg)

The big picture <font color="red">for an hypothesis driven, confirmatory study</font>
========================================================
transition: none
incremental: true

![](data-flow-steps-analysis-expanded-nopublication-02.svg)

# How does this compare to a pilot study or an exploratory study?

Pilot study
========================================================
transition: none
incremental: true

![](data-flow-steps-analysis-expanded-nopublication-02.svg)



Important side note
========================================================
type: prompt
incremental: true

As an example, consider a comparison of means between two groups.

<img src="slides-figure/unnamed-chunk-2-1.png" title="plot of chunk unnamed-chunk-2" alt="plot of chunk unnamed-chunk-2" style="display: block; margin: auto;" />

***

What is the interpretation if $\ p < 0.05$?

![](conclusive-difference.svg)

What is the interpretation if $\ p > 0.05$?

Important side note
========================================================
type: prompt
incremental: true

![](failure-to-show-difference-is-not-similarity.svg)

Important side note
========================================================
type: prompt
incremental: true

![](failure-to-show-difference-is-similarity-or-inconclusive.svg)

### It is a mistake to say: *There was no difference in mean Y between groups.*

### It is correct to say: *At the given sample size, a difference in mean Y was not detected.*

### It is cutting-edge to use **a second-generation p-value** and to prespecify a meaningful **null region**.


========================================================
type: prompt

<br><br><br>

## Important side note over


Back to the big picture
========================================================

## &nbsp;

![](data-flow-steps-analysis-expanded-nopublication-02.svg)


Big picture
========================================================

## Suppose one knew the truth

![](data-flow-steps-analysis-expanded-nopublication-03.svg)


Big picture
========================================================
incremental: true
<p></p>
## Suppose one repeated the study multiple times

![](data-flow-steps-analysis-expanded-nopublication-04.svg)

***

<p></p>
## Would one get the same result each time?

<br><br><br>

# **Probably** not

Key vocabulary
========================================================

# **Operating characteristic:**

## The distribution of a study trait over repeated executions of the study.

Types of study traits
========================================================

1. Sample size
1. False positive rate
1. False negative rate
1. False direction rate


Possible study traits
========================================================

1. Sample size
1. False positive rate  **(Type I error)**
1. False negative rate  **(Type II error)**
1. False direction rate  **(Type S error)**

Type I error
========================================================

![](data-flow-steps-analysis-expanded-nopublication-type-1-error.svg)

Type I error
========================================================

![](data-flow-steps-analysis-expanded-nopublication-type-1-error-02.svg)

Type I error
========================================================

![](data-flow-steps-analysis-expanded-nopublication-type-1-error-03.svg)

Type II error
========================================================

![](data-flow-steps-analysis-expanded-nopublication-type-2-error-01.svg)

Type II error
========================================================

![](data-flow-steps-analysis-expanded-nopublication-type-2-error-02.svg)

Type II error
========================================================

![](data-flow-steps-analysis-expanded-nopublication-type-2-error-03.svg)

Type II error
========================================================

![](data-flow-steps-analysis-expanded-nopublication-type-2-error-04.svg)

Operating characteristics
========================================================
incremental: true
<br><br>
## Who cares about **operating characteristics**?

### A **researcher** should understand the sample size needed for a study to generate conclusive results.

### Operating characteristics are helpful quantities for **grant reviewers** and **funding agencies** and anyone who must judge the likelihood that a study will generate conclusive results within budget.

### **Data scientists** calculate operating characteristics to understand the performance of a proposed analysis method.

Operating characteristics
========================================================
incremental: true
<br><br>
## When should we care about **power**?

### **Grant reviewers** generally prefer to fund projects that will lead to conclusive results.

### **Data scientists** prefer that study analysis plans use methods that maximize power.





Operating characteristics
========================================================
incremental: true
<br><br>
## When should we NOT care about **power**?

### **Grant reviewers** generally prefer to fund projects that will lead to conclusive results.

### **Data scientists** prefer that study analysis plans use methods that maximize power.

