---
layout: leap_day
usemathjax: true
---

# Computing


Here you can find some of my computing projects.



### COVID-19 Hospitalization Forecaster

Lara Du, Kai Wei and I built a machine learning tool to predict the number of hospital beds that
will be needed for COVID-19 patients in each state, up to 14 days in the future. Our prediction tool
comes with an API and a website, and comes in a docker container for easy deployment. The website for our
project is <a href="https://covidforecast.net" target="_blank">https://covidforecast.net</a>, and the GitHub repository with our code is at
<a href="https://github.com/czkaiweb/ErdosProject-COVID" target="_blank">https://github.com/czkaiweb/ErdosProject-COVID</a>.

---
### Dynamical imaging with interferometry

Very long baseline interferometry (VLBI) is a technique in which an array of telescopes around the globe
can be combined to function as a planet-sized telescope. The relative position of the telescopes changes as the planet
rotates, providing extra information. It is a difficult and mathematically interesting problem how to generate the most accurate possible image from the
available data, and the problem is made more difficult if the object being observed is changing over the course of the observation. I, along with several astronomers
working on the Event Horizon Telescope, developed an algorithm
to reconstruct a changing image (a "movie") from interferometric data.

Our research was published in the [Astrophysical Journal](https://doi.org/10.3847/1538-4357/aa97dd).


---
### Congruences modulo prime powers

Combinatorial sums often times satisfy interesting divisibility properties. For example, 
for every prime $$p\geq 7$$, the integer

$$\sum_{n=1}^p {p\choose n}{2p\choose n} + 6 - \frac{9}{2}{2p\choose p}$$

is divisible by $$p^5$$. I developed some algorithms for symbolically finding and proving identities like the
one above, and implemented them in Python. You can get the code at <a href="https://github.com/julianrosen/mhs" target="_blank">https://github.com/julianrosen/mhs</a>.

---
### Recurrence sequences

Suppose $$a_0,a_1,a_2,\ldots$$ is a sequence of integers satisfying a linear recurrence relation \\[a_{n} = c_1 a_{n-1} + \ldots + c_k a_{n-k}.\\]
The sequence of residue classes $$a_p \mod p$$ (as $$p$$ ranges through the prime numbers) has many interesting properties. For example:

- there is a non-zero polynomial $$f(x)$$ with integer coefficients (depending on the sequence but independent of $$p$$) with the property that $$f(a_p)\equiv 0\mod p$$
for every $$p$$, and
- the set of primes $$\{p:a_p\equiv 0\mod p\}$$ has rational natural density, and is in fact is a *Frobenian* set (this means there is a finite Galois extension
$$L/\mathbb{Q}$$ and a union of conjugacy classes $$S\subseteq\operatorname{Gal}(L/\mathbb{Q})$$ such that for $$p\gg0$$, $$a_p\equiv 0\mod p$$ if and only if the Frobenius at $$p$$ is in $$S$$).

These results and some others are proven in my paper [A finite analogue of the ring of algebraic number](pdf/Rosen_2020_A_finite_analogue_of_the_ring_of_algebraic_numbers.pdf).
I wrote software for performing symbolic calculations with linear recurrence sequences in SageMath, and for computing the polynomial $$f$$ and the extension $$L/\mathbb{Q}$$ and the set $$S\subset\operatorname{Gal}(L/\mathbb{Q})$$ appearing above. The code is
available at <a href="https://github.com/julianrosen/recurrence" target="_blank">https://github.com/julianrosen/recurrence</a>.

---
### Mudpi

Mudpi is a browser-based multiplayer online text adventure game that I put together during the pandemic in order to
keep in touch with some friends I could no longer visit with. Mudpi was originally served from a Raspberry Pi in
my home (whence the name), but now resides on a virtual private server. The game can be accessed 
at <a href="https://muttmutt.net/mudpi" target="_blank">https://muttmutt.net/mudpi</a>, and the source code can be found at
<a href="https://github.com/julianrosen/mudpi" target="_blank">https://github.com/julianrosen/mudpi</a>.

