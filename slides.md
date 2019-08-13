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
.reveal .fakeh2 {
font-size: 1.3em;
font-weight: bold;
}
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


========================================================

## The big picture

![](data-flow-steps-analysis-expanded-nopublication-01.svg)



========================================================

## The big picture for an **hypothesis driven, confirmatory study**

![](data-flow-steps-analysis-expanded-nopublication-01.svg)


========================================================

## The big picture **for an hypothesis driven, confirmatory study**

![](data-flow-steps-analysis-expanded-nopublication-02.svg)

========================================================

## The big picture **for an hypothesis driven, confirmatory study**

![](data-flow-steps-analysis-expanded-nopublication-02.svg)

## How does a **confirmatory study** compare to a **pilot study** or an **exploratory study**?

Hypothesis driven vs pilot study
========================================================

![](pilot-comparison.svg)

Hypothesis driven vs exploratory study
========================================================

![](exploratory-comparison.svg)

========================================================
<br><br><br>
# The **deliverables** of your proposed study should match the type of study you are performing

Deliverables
========================================================

| Pilot | Exploratory | Confirmatory |
|:-----:|:-----------:|:------------:|
| Demonstration of logistical capability | Hypotheses for future research | Tested hypotheses, usually resulting in |
| Collection of preliminary data | | + Conclusive difference |
| Go/No go decision about next stepᵃ | | + Conclusive similarity |
| | | + Inconclusive result |

ᵃ This is different from an hypothesis test

Helpful advice for pilot studies
========================================================

![](pilot-study-recommendations-paper.png)

========================================================

## For the remainder of the presentation, we are going to focus on hypothesis driven studies.

![](data-flow-steps-analysis-expanded-nopublication-02.svg)


========================================================
type: prompt
incremental: true

<div class="fakeh2">Important side note about hypothesis driven studies</div>
<br>
As an example, consider a comparison of means between two groups.

<img src="slides-figure/unnamed-chunk-2-1.png" title="plot of chunk unnamed-chunk-2" alt="plot of chunk unnamed-chunk-2" style="display: block; margin: auto;" />

***

<br><br><br>What is the interpretation if <br>p< 0.05?

![](conclusive-difference.svg)

What is the interpretation if <br>p > 0.05?

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

Note that the ? changes to A.

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

Big picture
========================================================
incremental: false
transition: none
<p></p>
## Suppose one repeated the study multiple times

![](data-flow-steps-analysis-expanded-nopublication-05.svg)

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
1. Cluster stability


Possible study traits
========================================================

1. Sample size
1. False positive rate  **(Type I error)**
1. False negative rate  **(Type II error)**
1. False direction rate  **(Type S error)**
1. Cluster stability

Type I error
========================================================

![](type-i-error-definition.svg)


Type I error
========================================================

![](type-i-error-definition-02.svg)


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

![](type-ii-error-definition-01.svg)


Type II error
========================================================

![](type-ii-error-definition-02.svg)


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

### After the data is collected.

### After the analysis has been performed.

Post-Hoc Power Is Not A Thing
========================================================

## Helpful resource: **DATAMETHODS.org**

![](post-hoc-power-is-not-a-thing.svg)

How to calculate power
========================================================

1. Simulation (prefered, for simple and complex study designs)
2. Calculators (for simple designs)


Simulation
========================================================

![](simulated-power-01.svg)

Simulation
========================================================

![](simulated-power-02.svg)

Simulation
========================================================

![](simulated-power-03.svg)

Simulation
========================================================

Needed Information:

1. Study design
1. Analysis plan
1. Approximate distribution of primary outcome
1. Approximate distribution of primary exposure
1. Parameters of interest (N, effect size, etc.)


Power calculators (for simple study designs)
========================================================

Needed Information:

1. Study design
1. Analysis plan
1. Mean and SD of primary outcome
1. Parameters of interest (N, effect size, etc.)

Online calculators (for simple study designs)
========================================================

1. Sealed Envelope: https://www.sealedenvelope.com/
1. SWOG Stat: https://stattools.crab.org/
1. Sample Size.net: https://www.sample-size.net/

How to present power
========================================================

## Fix N

<img src="slides-figure/unnamed-chunk-3-1.png" title="plot of chunk unnamed-chunk-3" alt="plot of chunk unnamed-chunk-3" style="display: block; margin: auto;" />

How to present power
========================================================

## Fix the effect size

<img src="slides-figure/unnamed-chunk-4-1.png" title="plot of chunk unnamed-chunk-4" alt="plot of chunk unnamed-chunk-4" style="display: block; margin: auto;" />

How to present power
========================================================

## Fix the power

<img src="slides-figure/unnamed-chunk-5-1.png" title="plot of chunk unnamed-chunk-5" alt="plot of chunk unnamed-chunk-5" style="display: block; margin: auto;" />

Hands-on (simple study designs)
========================================================

1. **How many** subjects are required to have a 90% chance of detecting, as significant at the 5% level, a decreased mortality rate from 45% in the control group to 25% in the experimental group.

2. With 25 subjects in each group, **what is the minimal detectable difference** in mean creatinine at 90% power when α = 0.05 and SD = 1.
