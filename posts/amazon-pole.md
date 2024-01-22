---
title: 'The Amazon Hanging Cable Problem'
date: '2023-02-26'
---

The Amazon Hanging Cable Problem has been supposedly asked in their job interviews and it has circulated the internet for a while now.

![Image of the hanging cable problem](/images/pole.png)

The problem shows two **50m** tall poles separated by a distance **x**. The poles are interconnected by an **80m** long cable which hangs **10m** above the ground.  We have to find the distance **x**.

I could not solve this problem on my own and had to resort to a video which shows a simple logical solution. It demonstrates that the only way the above described scenario can happen is if the poles are directly touching each other, i.e. **x = 0m**. Anyone can easily see that after the idea is revelaed, you just picture that the cable goes down for **40m** along the first pole and **40m** up along the second pole, and at the lowest point it is **10m** from the ground.

That is nice, but I have been wondering if it's possible to model the height of the midpart of the cable **h(x)** as a function of the distance between the poles, or vice-versa, **h-¹(x) = d(x)**.

We already know from the logical solution that:

- **h(0) = 10m**;
- **h(80) = 50m**.

And that **x ∈ ℝ | 0 ≤ x ≤ 80m**.

Luckily, because the math is heavy and involves hyperbolic trigonometric functions and something called catenary which I've never heard of, I found a paper by Chatterjee, Neil and Bogdan G. Nita called *["The hanging cable problem for pratical applications"](http://euclid.trentu.ca/aejm/V4N1/Chatterjee.V4N1.pdf)*, which does most of the work for me.

From the equation **(17)** on page 4, with adaptations, it follows that:

![Image of function d(x)](/images/dx.png)

With the following plot:

![Image of plot of function d(x)](/images/dxplot.png)

Note that the above plot is only valid for **x ∈ ℝ | 10 ≤ x ≤ 50m**, the domain of **d(x)**.

That looks somewhat like a log curve, which seems reasonable. I don't know what I was expecting to see. To find the **h(x)** and its plot, just invert that function, it is left as an exercise to the reader.