---
title: grad.desc()
subtitle: Demonstration of the Gradient Descent Algorithm
date: '2017-04-04'
slug: grad-desc
from_Rmd: yes
---

This function provids a visual illustration for the process of minimizing a
real-valued function through Gradient Descent Algorithm.

Gradient descent is an optimization algorithm. To find a local minimum of a
function using gradient descent, one takes steps proportional to the negative
of the gradient (or the approximate gradient) of the function at the current
point. If instead one takes steps proportional to the gradient, one
approaches a local maximum of that function; the procedure is then known as
gradient ascent.

The arrows are indicating the result of iterations and the process of
minimization; they will go to a local minimum in the end if the maximum
number of iterations `ani.options('nmax')` has not been reached.
 

```r
library(animation)
## default example
ani.options(interval = 0.3, nmax = 50)
xx = grad.desc()
```

```r
xx$par  # solution
```

```
##          x          y 
## -0.0675852  0.0009736
```

```r
xx$persp(col = "lightblue", phi = 30)  # perspective plot
```

<video controls loop autoplay><source src="https://assets.yihui.org/figures/animation/example/grad-desc/demo-a.mp4" /><p>plot of chunk demo-a</p></video>

```r
## define more complex functions; a little time-consuming
f1 = function(x, y) x^2 + 3 * sin(y)
xx = grad.desc(f1, pi * c(-2, -2, 2, 2), c(-2 * pi, 2))
```

```r
xx$persp(col = "lightblue", theta = 30, phi = 30)
```

<video controls loop autoplay><source src="https://assets.yihui.org/figures/animation/example/grad-desc/demo-b.mp4" /><p>plot of chunk demo-b</p></video>


```r
## need to provide the gradient when deriv() cannot handle the
## function
grad.desc(FUN = function(x1, x2) {
  x0 = cos(x2)
  x1^2 + x0
}, gr = function(x1, x2) {
  c(2 * x1, -sin(x2))
}, rg = c(-3, -1, 3, 5), init = c(-3, 0.5), main = expression(x[1]^2 + 
  cos(x[2])))
```

```
## Warning in grad.desc(FUN = function(x1, x2) {: Maximum
## number of iterations reached!
```

<video controls loop autoplay><source src="https://assets.yihui.org/figures/animation/example/grad-desc/demo-c.mp4" /><p>plot of chunk demo-c</p></video>


```r
## or a even more complicated function
ani.options(interval = 0, nmax = 200)
f2 = function(x, y) sin(1/2 * x^2 - 1/4 * y^2 + 3) * cos(2 * 
  x + 1 - exp(y))
xx = grad.desc(f2, c(-2, -2, 2, 2), c(-1, 0.5), gamma = 0.1, 
  tol = 1e-04)
```

<video controls loop autoplay><source src="https://assets.yihui.org/figures/animation/example/grad-desc/demo-d.mp4" /><p>plot of chunk demo-d</p></video>


```r
## click your mouse to select a start point
if (interactive()) {
  xx = grad.desc(f2, c(-2, -2, 2, 2), interact = TRUE, tol = 1e-04)
  xx$persp(col = "lightblue", theta = 30, phi = 30)
}
```
