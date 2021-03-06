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

We can create a dummy variable a that is 1 if the responder accepts the offer and 0 if the responder rejects the offer. 

Using this we can create a best response function $U_R = a(t)$

Once the responder knows the value of t given by the proposer, he can pick the value of a to maximize the best response function, which will be accepting any t>0 and being indifferent when t=0.

### Question 2

Given that best response function, the proposer gets utility

$U_P = a(x-t)$ 

We know the value of a will be 1 if t>0, and since the responder would be indifferent if t=0, we assume that they would randomize with equal probability between accepting and rejecting. That means if t=0, then $U_P = .5(x)$ and if t>0 then $U_P = x-t$

If t>0, a will always be 1, and the proposer should try to minimize t. In this case, the minimal value of t where t>0 would be t=1.

So given the value of x, the proposer should pick the maximum of $.5(x)$ and $x-t$ to decide what they should do.

### Question 3

$\epsilon$ represents the players greed/desire to end up with more than the opposing player. If $\epsilon = 0$ then the player doesn't care about that at all.

$\gamma$ represents the players guilt/desire for fairness if they end up with more than the opposing player. If $\epsilon = 0$ then the player doesn't care about that at all.

### Question 4

If the responder accepts the offer their utility function would be
$U_r = X_r - \frac{3}{4}Max(0, X_p-X_r) - \frac{1}{6}Max(0,X_r - X_p)$

If the responder rejects the offer their utility function would be 
$U_r = 0 - \frac{3}{4}0 - \frac{3}{4}0 = 0$

Therefore if the responder gets a utility of U>0 by accepting the offer, they should accept, and if they get a U<0 by rejecting the offer, they should reject. We create a dummy variable a that is 1 if the responder accepts and 0 if the responder rejects. Then we can write the responders best response function as $U_r = a(X_r - \frac{3}{4}Max(0, X_p-X_r) - \frac{1}{6}Max(0,X_r-X_p))$. The responder would then maximize $U_r$ given $X_r$ and $X_p$ by deciding a.

The best incentive for the proposer is to offer the smallest amount that the responder would accept. We know that the proposer would get 0 if the deal was rejected so the proposer wants to make sure the deal is accepted. We know that he should offer the smallest amount the responder would accept by looking at his utility function $U_p = X_p - \frac{3}{4}Max(0,X_r - X_p) - \frac{1}{6}Max(0, X_p-X_r)$. We can see that the proposer loses some utility by getting more money than the responder, but not as much utility as he gains from getting the extra money. Increasing $X_r$ by 1 (by decreasing $X_p$ by 1) would increase the last term of the utility function by 2/6, but would also decrease the first term by 1, so the proposer loses utility for every dollar he gives away.

We can find the smallest amount the responder would accept by setting a in his best response function to 1 (because we want to make sure he accepts), then setting the function equal to 0 (where he would be indifferent between accepting and rejecting). Once we find the proposal he'd be indifferent on, we would propose the smallest amount above that # that we could (to make sure he accepts).

Setting a in the responders best response function gives us $U_r = X_r - \frac{3}{4}Max(0, X_p-X_r) - \frac{1}{6}Max(0,X_r-X_p)$. We know that the proposer wants to maximize his money, and the responders $\epsilon$ is less than 1 (meaning he values receiving a dollar more than he is negatively impacted by having less than the other player). This means that we know $X_p$ will be greater than $X_r$, and we can therefore discard the last term of the responders BR function.

We now have $U_r = X_r - \frac{3}{4}Max(0, X_p-X_r)$. Since we know that $X_p > X_r$ and therefore $X_p - X_r >0$, we can further simplify to $U_r = X_r - \frac{3}{4}(X_p-X_r) = \frac{7}{4}X_r - \frac{3}{4}X_p$, which we can set equal to 0. 

Assuming the proposer has 48 dollars to split, we can rewrite again to $0=\frac{7}{4}(48-X_p) - \frac{3}{4}X_p = 84 - \frac{7}{4}X_p - \frac{3}{4}X_p = 84 - \frac{5}{2}X_p$ or $\frac{5}{2}X_p = 84$ which simplifies to $X_p = 33.6$ which corresponds with $X_r = 48-33.6 = 14.4$.

Since the responder would be indifferent between accepting and rejecting when the offer was 14.4, the proposers best move would be to offer 15 dollars.
