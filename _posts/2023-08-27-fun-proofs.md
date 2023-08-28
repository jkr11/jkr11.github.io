---
layout: post
title: Fun proofs
latex: true
---

This entry contains a list of proofs i found that either support my studies or were interesting/unique enough to write down.


<!--more-->



**Theorem 1**. *Fermat's (little) Theorem*

*For all $$a \in \mathbb{Z}$$ and every Prime $$p$$ there is:
$$a^p = a \mod p \iff p \mid a^p - a$$*

*Proof.* {% include sidenote.html note="Side note: After [Lionel Levine](https://pi.math.cornell.edu/~levine/fermat.pdf), Math. Magazine 1999." %}

For all $$a \geq 2$$ and $$p$$ prime, let $$f: \mathbb{C} \to \mathbb{C}$$ be
defined by $$f(z) = z^a$$. It's pth iterate is $$f_p(z) = z^{a^p}$$. Let
$$S_p$$ be the Set of all $$z$$ s.t. they are fixed under $$f_p$$ but not $$f$$
itself, i.e: $$S_p = \{z \in \mathbb{C}: f_p(z) = z, f(z) \neq z\},$$
meaning all $$s \in S_p$$ satisfy $$z^{a^p} - z = 0$$ and $$z^a - z \neq 0$$,
having $$a^p$$ and $$a$$ respective roots. Thus the cardinality
$$\left\vert S_p  \right\vert = a^p - a$$. But for all $$z \in S_p$$ and the
$$p$$ numbers $$f(z), f_1(z) , \ldots , f_{p-1} (z)$$ are all distinct (due
to $$p$$ prime). Therefore, $$S_p$$ can be partitioned in $$p$$-equivalence
classes, giving $$p \mid a^p - a$$ ◻

