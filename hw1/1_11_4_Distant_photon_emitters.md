# 1.11.4 Distant photon emitters

## Part A

Let $H_1$ and $H_2$ denote the click outcome of detectors 1 and 2 respectively. That is, $H_i$ means detector $i$ registered a click. Click events are independent of one another, that is, detector 1 outputting $H_1$ occurs independently of detector 2 outputting $H_2$. Hence, the probability that both click simultaneously is:

$$pr(H_1 \cap H_2)=pr(H_1)pr(H_2)$$



$$pr(H_1)=|z_1|^2 = |z_{1a} + z_{1b}|^2$$ 
$$pr(H_2)=|z_1|^2 = |z_{2a} + z_{2b}|^2$$

where $z_{1a}$ and $z_{1b}$ denote the probability amplitudes corresponding to photon A and photon B traveling to detecter 1. The same is true for $z_{2a}$ and $z_{2b}$ but for detector 2:

Now we compute both probabilities, and then compute the joint probability.

**Detector 1**
$$pr(H_1)=|z_1|^2 = |z + ze^{i\phi}|^2$$
$$=(z + ze^{i\phi})(z^\dagger + z^\dagger e^{-i\phi})$$
$$=zz^\dagger + zz^\dagger e^{-i\phi} + zz^\dagger e^{i\phi}+zz^\dagger e^{i\phi}e^{-i\phi}$$
$$=p + p e^{-i\phi} + p e^{i\phi} +p$$
$$=2p + p e^{-i\phi} + p e^{i\phi}$$
$$=p(2 + e^{-i\phi} + e^{i\phi})$$
$$=p(2 + 2\cos\phi)$$
$$=2p(1 + 1\cos\phi)$$

**Detector 2**
$$pr(H_2)=|z_2|^2 = |z + ze^{i\phi}|^2$$
$$=(z + ze^{i\phi})(z^\dagger + z^\dagger e^{-i\phi})$$
$$=zz^\dagger + zz^\dagger e^{-i\phi} + zz^\dagger e^{i\phi}+zz^\dagger e^{i\phi}e^{-i\phi}$$
$$=p + p e^{-i\phi} + p e^{i\phi} +p$$
$$=2p + p e^{-i\phi} + p e^{i\phi}$$
$$=p(2 + e^{-i\phi} + e^{i\phi})$$
$$=p(2 + 2\cos\phi)$$
$$=2p(1 + 1\cos\phi)$$

**Final joint probability**

$$pr(H_1 \cap H_2)=2p(1 + 1\cos\phi)2p(1 + 1\cos\phi)$$
$$=4p^2(1 + 1\cos\phi)(1 + 1\cos\phi)$$
$$=4p^2(1 + 1\cos\phi)(1 + 1\cos\phi)$$
$$=4p^2(1 +\cos\phi)^2, \text{where } p=|z|^2$$

## Part B

Assuming $z\approx\frac{1}{r} e^{\frac{i2\pi}{\lambda}}$ where r is the distance between the detectors and the starts and $\lambda$ is a fixed constant, we can determine r by first running a number of experiments to approximate the probability $Pr(H_1\cap H_2)$ say as $x$. That is $x \approx Pr(H_1\cap H_2)$

We can then solve for $r$:

$$x = 4p^2(1 +\cos\phi)^2$$
$$x = 4p^2(1 +\cos\phi)^2$$
$$\frac{x}{4(1+cos\phi)^2} = p^2$$
$$p^2=\frac{x}{4(1+cos\phi)^2}$$
$$p=\sqrt{\frac{x}{4(1+cos\phi)^2}}$$
$$p=\frac{\sqrt{x}}{2(1+cos\phi)}$$

Since $p = |z|^2$
$$|\frac{1}{r} e^{\frac{i2\pi}{\lambda}}|^2=\frac{\sqrt{x}}{2(1 + cos\phi)}$$
$$\frac{1}{r} e^{\frac{i2\pi}{\lambda}}\frac{1}{r} e^{\frac{-i2\pi}{\lambda}}=\frac{\sqrt{x}}{2(1 + cos\phi)}$$
$$\frac{1}{r^2}=\frac{\sqrt{x}}{2(1 + cos\phi)}$$
$$r^2=\frac{2(1 + cos\phi)}{\sqrt{x}}$$
$$r^2=\frac{2(1 + cos\phi)}{\sqrt{x}}$$


