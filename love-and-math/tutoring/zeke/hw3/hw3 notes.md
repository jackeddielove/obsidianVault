[[hw3.pdf]]

Use the integral test, and the fact that
$$\int\frac{1}{x\sqrt{x^2-1}}dx=\sec^{-1}x+C$$
to show that
$$\sum_{n=2}^\infty \frac{1}{n\sqrt{n^2-1}}$$
converges.
$$\int_2^b\frac{1}{x\sqrt{x^2-1}}dx=\sec^{-1}x\vert_2^b$$
$$\int_2^\infty\frac{1}{x\sqrt{x^2-1}}dx=\lim_{b\to\infty}\sec^{-1}x\vert_2^b$$
$$=\lim_{b\to\infty}\sec^{-1}b-\sec^{-1}2$$
$$=\frac{\pi}{2}-\frac{\pi}{3}=\frac{\pi}{6}$$


Find $N$ such that $R_N\leq0.01$.

Remainder theorem:
$$\int_{n+1}^\infty f(x)\, dx \leq R_n \leq \int_n^\infty f(x)\, dx$$

From above, we have

$$\int_a^\infty\frac{1}{x\sqrt{x^2-1}}dx=\frac{\pi}{2}-\sec^{-1}a$$
so we want to find $a$ such that $\frac{\pi}{2}-\sec^{-1}a\leq0.01$.
$$\begin{align}
\frac{\pi}{2}-\sec^{-1}a=0.01 &\Rightarrow \sec^{-1}a=\frac{\pi}{2}-0.01 \\
&\Rightarrow a=\sec(\frac{\pi}{2}-0.01) \\
&\Rightarrow a\approx 100
\end{align}$$
[Desmos](https://www.desmos.com/calculator/vyd8lqwclc)
$$\sum_{n=2}^{101}(\frac{1}{n\sqrt{n^2-1}})\approx 0.68$$


$$\sum_{n=1}^{764}(\frac{\ln n}{n^2})$$
