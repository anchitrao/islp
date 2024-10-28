# Exercise 3

Here's the proof with cleaned up formatting, maintaining consistent spacing and alignment:

$$
p_k(x)=\frac{\pi_k\frac{1}{\sqrt{2\pi}\sigma}\exp(-\frac{1}{2\sigma^2}(x-\mu_k)^2)}{\sum_{l=1}^{K}\pi_l\frac{1}{\sqrt{2\pi}\sigma}\exp(-\frac{1}{2\sigma^2}(x-\mu_l)^2)}
$$

$\text{argmax}$ of a function is unchanged by $\log$ as it is a monotonic function.

$$
\text{argmax}_k(p_k(x))=\text{argmax}_k(\log(p_k(x)))
$$

$$
\log(p_k(x))=\log(\pi_k)+\log(\frac{1}{\sqrt{2\pi}\sigma})-\frac{1}{2\sigma^2}(x-\mu_k)^2-\log(\sum_{l=1}^{K}\pi_l\frac{1}{\sqrt{2\pi}\sigma}\exp(-\frac{1}{2\sigma^2}(x-\mu_l)^2))
$$

Denominator sum term is constant with respect to $k$, so it can be ignored. $\log(\frac{1}{\sqrt{2\pi}\sigma})$ is constant across all $k$ under our assumption that $\sigma_1^2=\dots=\sigma_k^2$, so it can also be ignored.

$$
\text{argmax}_k(p_k(x))=\text{argmax}_k(\log(\pi_k)-\frac{1}{2\sigma^2}(x-\mu_k)^2)
$$

$$
=\text{argmax}_k(\log(\pi_k)-\frac{1}{2\sigma^2}(x^2-2x\mu_k+\mu_k^2))
$$

$x^2/2\sigma^2$ is constant with respect to $k$, so it can be ignored.

$$
=\text{argmax}_k(x\frac{\mu_k}{\sigma^2}-\frac{\mu_k^2}{2\sigma^2}+\log(\pi_k))
$$

$$
\delta_k(x)=x\frac{\mu_k}{\sigma^2}-\frac{\mu_k^2}{2\sigma^2}+\log(\pi_k)
$$

Therefore,

$$
\text{argmax}_k(p_k(x))=\text{argmax}_k(\delta_k(x))
$$


WORK IN PROGRESS