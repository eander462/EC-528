---
title: "HW4"
author: "Erik Andersen, Jeremy Patak"
date: '2022-05-25'
output: 
  html_document:
    toc: true
    toc_float: true
    keep_md: yes
---



### Question 1

The responder gets 0 utility if they reject the offer, and t utility if they accept it where t is the amount the propoeser proposes. So to maximize utility, the responder's best response function is to choose to accept the proposal when X-t>0 and reject otherwise.

In math their utility is:

$U_R$ = t if t > 0 

$U_R$ = 0 if t <= 0

Accept the offer if $U_R > 0$.

### Question 2

Given that best response function, the proposer gets utility

$U_P$ = X - t, if t > 0

$U_P$ = 0, if t <= 0

So to maximize their utility, they should choose the smallest possible t. If t is any positive number, the responder will accept the offer, and the smallest possible t means X - t is as large as possible. 
