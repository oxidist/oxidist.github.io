---
layout: post
comments: false
title: "The class number formula"
tags: mathematics
---
# Introduction
Recently, I came across a theorem which relates unique factorisation in a ring to the value of a certain $$\zeta$$ function. It also helps in determining whether the ring has unique factorisation if you can calculate the value of that $$\zeta$$ function.[^0]

I was quite impressed by this extraordinary connection between algebra and analysis, and wrote a short note on it for two of my friends which is reproduced here.

[^0]: And you don't need to have an exact value either, sometimes you can even approximate it.

# Fields

Let $$K = \mathbb{Q}(\sqrt{m} )$$ where $$m < 0$$ is square-free. This is known as an imaginary quadratic field, since it is a degree 2 extension of $$\mathbb{Q}$$, given by $$K = \mathbb{Q}[x]/(x^2 - m)$$.

It also has a *ring of integers* $$\mathcal{O}_K$$, which is the analogue of $$\mathbb{Z}$$ for this field. 
In fact, $$\mathcal{O}_K$$ is the [integral closure](https://en.wikipedia.org/wiki/Integral_element#Integral_closure_in_algebraic_number_theory) of $$\mathbb{Z}$$ in $$K$$.
Unfortunately, the ring $$\mathcal{O}_K$$ is not always a unique factorisation domain. 
For example, in $$\mathbb{Z}[\sqrt{-5}]$$ we have $$6 = 2 \cdot 3 = (1 + \sqrt{-5})(1 - \sqrt{-5})$$.
The *class number* measures how much $$\mathcal{O}_K$$ fails to be a principal ideal domain, and hence a unique factorisation domain.[^1]

[^1]: It is the order of a certain group known as the ideal class group. When the order is 1, $$\mathcal{O}_K$$ is a principal ideal domain.

Now, let 
$$N = \begin{cases} |m| & \text{if } m \equiv 1 \mod{4} \\ 
4|m| & \text{if } m \equiv 2,3\mod{4} \end{cases}$$

The number $$N$$ is known as the *discriminant* of the number field. 
We can define a group homomorphism $$\chi : (\mathbb{Z}/N\mathbb{Z})^\times \to \{\pm 1\} $$ as follows:
for any prime $$p$$ not dividing $$m$$, we put $$\chi(p) = \left( \frac{m}{p} \right) $$
  (This is the Legendre symbol, which outputs $$1$$ if  $$m$$ has a square root in  $$\mathbb{F}_p$$ and $$-1$$ otherwise).

# L functions
  We then form the series
  \\[
    L(s,\chi) = \sum_{n=1}^{\infty} \frac{\chi(n)}{n^s}.
  \\]
  where $$\chi(n)$$ is simply $$\chi(n \mod N)$$ if  $$n$$ is coprime to $$N$$ and 0 otherwise. 
  This type of series, which can be formed for any homomorphism $$\chi : (\mathbb{Z}/n\mathbb{Z})^\times \to \mathbb{C}^\times$$, is known as an $$L$$-function and is an extension of the Riemann $$\zeta$$ function.

  For example, if $$m = -1$$, then $$N=4$$ and we have $$\chi(1 \mod 4) = 1$$ and $$\chi(3 \mod 4) = -1$$. So, \\[L(1,\chi) = 1 - \frac{1}{3} + \frac{1}{5} - \frac{1}{7} + \dots = \arctan(1) = \frac{\pi}{4}.\\]

# The theorem 
  Here is the main theorem, known as the class number formula for quadratic imaginary fields.
> For an imaginary quadratic field $$K$$, let $$h_K$$ be its class number and $$w_K$$ the number of roots of $$1$$ in $$K$$. Then:
\\[h_K = \frac{w_K}{2} L(0,\chi) = \frac{w_K \sqrt{N} }{2\pi} L(1,\chi).\\]

That is to say, whether or not the ring of integers is a principal ideal domain depends on the value of a certain $$\zeta$$ function. 
That is strange and amazing.

For example, let's again take $$m = -1$$, so  $$K = \mathbb{Q}(\sqrt{-1} )$$. 
The roots of unity in this field are $$1, -1, \sqrt{-1}$$, and $$-\sqrt{-1}$$, so $$w_k = 4$$.
Using the theorem, we get:
 \\[
   h_K = \frac{w_K \sqrt{N}}{2\pi} L(1,\chi) = \frac{4 \cdot 2}{2\pi} L(1,\chi) = \frac{4}{\pi} \cdot L(1,\chi)
\\]
Here $$L(1,\chi) = 1 - \frac{1}{3} + \frac{1}{5} - \dots = \frac{\pi}{4}$$, so $$h_K = 1$$.
Therefore $$\mathcal{O}_K = \mathbb{Z}[\sqrt{-1}]$$ is a principal ideal domain.
It is striking that we took a detour through analysis to prove an algebraic fact!

---
