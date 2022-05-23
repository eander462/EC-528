---
title: "HW3"
author: "Jeremy Patak"
date: '2022-05-15'
output: 
  html_document:
    toc: true
    toc_float: true
    keep_md: yes
---

### Question 1

#### 1.1
$U(c_1, c_2, c_3) = log(c_1) + \delta log(c_2) + \delta^2log(c_3)$

#### 1.2
$M_1 + \frac{M_2}{1+r} + \frac{M_3}{(1+r)^2} = c_1 + \frac{c_2}{1+r} + \frac{c_3}{(1+r)^2}$

#### 1.3
We'll do this with the lagrange method

First, we set up the lagrangian:

$L = log(c_1) + \delta log(c_2) + \delta^2log(c_3) - \lambda (M_1 + \frac{M_2}{1+r} + \frac{M_3}{(1+r)^2} = c_1 + \frac{c_2}{1+r} + \frac{c_3}{(1+r)^2})$

Then differentiate by each variable

$dL/dc_1 = 1/c_1 - \lambda = 0$

$dL/dc_2 = \delta/c_2 - \lambda/(1+r) = 0$

$dL/dc_3 = \delta^2/c_3 - \lambda/(1+r)^2 = 0$

We know that the marginal utility for $c_t$ is $U'(c_t) = 1/c_t$ so we can plug that into the equations we just got:

$dL/dc_1 = U'(c_1) - \lambda = 0$

$dL/dc_2 = \delta U'(c_2) - \lambda/(1+r) = 0$

$dL/dc_3 = \delta^2 U'(c_3) - \lambda/(1+r)^2 = 0$

Now simplify

$U'(c_1) = \lambda$

$U'(c_2)\delta(1+r) = \lambda$

$U'(c_3)\delta^2(1+r)^2 = \lambda$

Now we can equate them since they all equal $\lambda$

$U'(c_1) = \delta (1+r)U'(c_2) = \delta^2 (1+r)^2 U'(c_3)$


#### 1.4

To solve this question, we will take the relationship we solved for in the previous step, plug in the values for delta and r we are given, then solve each in terms of c1. We will then plug each into the budget constraint to solve for the optimum consumption quantities. 

$U'(c_1) = 1/c_1$

$1/c_1 = .95(1.05)/c_2$

$c_1 = c_2 / .95*1.05$

$c_2 = .95*1.05c_1$

Now c3

$1/c_1 = .95^2(1.05^2)/c_3$

$c_1 = c_3/.95^2*1.05^2$

$c_3 = .95^2*1.05^2c_1$

Now we plug these values into the budget constraint.

$M_1 + \frac{M_2}{1+r} + \frac{M_3}{(1+r)^2} = c_1 + \frac{c_2}{1+r} + \frac{c_3}{(1+r)^2}$

$100(1 + 1/1.05 + 1/1.05^2) = c_1 + .95*1.05c_1/1.05 + .95^2*1.05^2c_1/1.05^2$

$285.94 = c_1 + .95c_1 + .95^2c_2$

$285.94 = 2.85c_1$

$c_1 = 100.24$

Plug that into the equations for c2 and c3.

$c_2 = .95*1.05*100.24$

$c_2 = 99.99$

$c_3 = .95^2*1.05^2*100.24$

$c_3 = 99.74$

#### 1.5

We will repeat the same process as the previous question except for the second and third periods, we replace delta = .95 with delta = .95*.9 = .885. 

$1/c_1 = .95*.9(1.05)/c_2$

$c_1 = c_2 / .885*1.05$

$c_2 = .885*1.05c_1$

Now c3

$1/c_1 = .885^2(1.05^2)/c_3$

$c_1 = c_3/.885^2*1.05^2$

$c_3 = .885^2*1.05^2c_1$

Plug these new values for c2 and c3 into the budget constraint.

$100(1 + 1/1.05 + 1/1.05^2) = c_1 + .885*1.05c_1/1.05 + .885^2*1.05^2c_1/1.05^2$

$285.94 = c_1 + .885c_1 + .885^2c_2$

$285.94 = 2.668c_1$

$c_1 = 107.17$

$c_2 = .885*1.05*107.17$

$c_2 = 99.58$

$c_3 = .885^2*1.05^2*107.17$

$c_3 = 92.54$


### Question 2

#### 2.1
The standard model uses the expected utility theory, but this is violated in this example by the certainty effect. Winning the lottery is a very low probability outcome, so they will be more risk loving in this situation. However, making money off of bonds has a much higher probability, and the couple therefore displays risk aversion in that situation. This behavior is explained by the certainty effect, but not by the standard model.

#### 2.2
This behavior is likely a form of default options. People don't know how much they want to save, so they pick an option that has significance from the employer or government (max amounts matches, etc.). If that is why people are making this choice, it violates the standard model, because the standard model assumes people have complete preferences and relying on the default option breaks that assumption. 
