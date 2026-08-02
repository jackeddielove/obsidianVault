

The alternating series test:
If $a_{n+1}\leq a_n$ and $\lim_{n\to\infty}a_n=0$, then $\sum (-1)^n a_n$ converges.

Example: $$\sum \frac{(-1)^n}{n}$$
# 1
The series
$$\sum \frac{(-1)^n\ln n}{n}$$
converges by the alternating series test, but
$$\sum \bigg|\frac{(-1)^n\ln n}{n}\bigg|=\sum \frac{\ln n}{n}$$
diverges by the direct comparison test with the harmonic series. Thus our series converges conditionally.
# 2
The series $$\sum \frac{(−1)^{k+1}}{\ln(\ln(k))}$$
converges by the alternating series test, but  $$\sum \frac{1}{\ln(\ln(k))}$$
diverges by the direct comparison test with the harmonic series. Thus our series converges conditionally.
# 3

$$\sum \frac{2^n}{n!}$$
Ratio test: Let  $L=\lim\bigg|\frac{a_{n+1}}{a_n}\bigg|$. If $L<1$ the series converges absolutely, if $L>1$, the series diverges, and if $L=1$ the test is inconclusive.

$$L=\lim_{n\to\infty}\bigg|\frac{\frac{2^{n+1}}{(n+1)!}}{\frac{2^n}{n!}}\bigg|=\lim_{n\to\infty}\frac{2^{n+1}n!}{2^n(n+1)!}=\lim_{n\to\infty}\frac{2}{n+1}=0$$
so the series converges absolutely.
# 4
$$\sum \left(\frac{2n+1}{3n+2}\right)^n$$
Root test: Let  $L=\lim\sqrt[n]{|a_n|}$. If $L<1$ the series converges absolutely, if $L>1$, the series diverges, and if $L=1$ the test is inconclusive.

$$L=\lim_{n\to\infty}\sqrt[n]{\left(\frac{2n+1}{3n+2}\right)^n}=\lim_{n\to\infty}\frac{2n+1}{3n+1}=\frac{2}{3}$$
so the series converges absolutely.
# 5

# 13
Show that if $$\lim_{n\to\infty}\frac{a_{n+1}}{a_n}<1$$
then there is a $r<1$ and an $N\in\mathbb{N}$ such that $$\frac{a_{n+1}}{a_n}\leq r$$
whenever $n>N$.

## a)
Show that when $n\geq N$, $a_n\leq a_Nr^{n-N}$.

$$\ldots a_{N-3}, a_{N-2}, a_{N-1}, a_N, a_{N+1}, a_{N+2}, a_{N+3}, \ldots$$
Notice that since$$\frac{a_{n+1}}{a_n}\leq r$$
, then $$a_{n+1}\leq a_nr$$