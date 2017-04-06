---
layout: page
permalink: /glossary/spheres/
title: "Spheres"
---


The implict equation for a sphere is:

$$x^2 + y^2 + z^2 - r^2 = 0$$

where `r` is the radius of the sphere.

Assuming the sphere has some center (offset) `cx, cy, cz`, then the implicit equation can be:


$$(x - cx)^2 + (y - cy)^2 + (z - cz)^2 - r^2 = 0$$

Using the equation of a ray:

$$p(t) = p0 + t * d$$

We want to solve for any values of `t` that are points on the sphere.

First we write the sphere equation in vector form (using vector dot product):

$$(p - c) \cdot (p - c) - r^2 = 0$$

Now, plug in our ray equation for p:

$$(p0 + t*d - c) \cdot (p0 + t*d - c) - r^2 = 0$$

If we can rearrange these terms to look like a quadratic equation ($$At^2 + Bt + C = 0$$) then we can use the quadratic equation to solve for t.

Consider:

$$((p0 - c) + t*d) \cdot ((p0 - c) + t*d) - r^2 = 0$$

Multiply the first two quantities (this may seem confusing because it's vectors)

$$(p0 - c) \cdot (p0 - c) + 2 (p0 - c) \cdot t * d + (d \cdot d) t^2 - r^2 = 0$$

or... (rearrange terms)

$$d^2 t^2 + 2 d \cdot (p0 - c) t + (p0 - c)^2 - r^2 = 0$$

(Note that any time we use $$v^2$$ for some vector v we mean $$v \cdot v$$)

Now we have a quadratic equation with the following parts:

$$ A = d \cdot d $$

$$ B = 2 d \cdot (p0 - c) t$$

$$ C = (p0 - c) \cdot (p0 - c) - r^2 $$

<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
