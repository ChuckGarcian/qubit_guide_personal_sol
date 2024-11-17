
# Converting 1 + eipsi to polar

**Claim:** Given the complex number $z = 1 + e^{i\theta}$, we claim:

$$
z = 1 + e^{i\theta} = 2\cos {\frac{\theta}{2}}e^{i\frac{\theta}{2}}
$$

**Proof:**

We will show the claim by showing there exist $(r, \phi)$ such that $z=re^{i\phi}=2\cos {\frac{\theta}{2}}e^{i\frac{\theta}{2}}$. In other words, $z$ in exponential form with $r=2\cos\frac{\theta}{2}$ and angle $\phi=\frac{\theta}{2}$.

$z = (x,y)$, we want $r$ and $\theta$ such that $z=(x,y)=(r\cos\theta, r\sin\theta)$.

**Find $r$:**

$$r = |z|$$

The modulus of a complex number is the length in Euclidean space. So take the square root of the product of the complex number and its conjugate:

$$=\sqrt{(1+e^{i\theta})(1+e^{-i\theta})}$$
$$=\sqrt{1 + e^{-i\theta} + e^{i\theta} + e^{i\theta}e^{-i\theta}}$$
$$=\sqrt{1 + e^{-i\theta} + e^{i\theta} + 1}$$
$$=\sqrt{2 + e^{-i\theta} + e^{i\theta}}$$

Use Euler's formula for $e$'s:

$$=\sqrt{2 + \cos\theta + i\sin\theta + \cos\theta - i\sin\theta}$$
$$=\sqrt{2 + \cos\theta + \cos\theta + i\sin\theta - i\sin\theta}$$
$$=\sqrt{2 + 2\cos\theta}$$
$$=\sqrt{2} \sqrt{1 + \cos\theta}$$

Use the trigonometric double angle identity $2\cos^2\frac{\theta}{2} = 1 + \cos\theta$:

$$=\sqrt{2} \sqrt{2\cos^2\frac{\theta}{2}}$$
$$=\sqrt{2} \sqrt{2}\sqrt{\cos^2\frac{\theta}{2}}$$
$$=2\cos\frac{\theta}{2}$$

So $r=2\cos\frac{\theta}{2}$.

**Find** $\mathbf{\phi}:$

$$z= r\cos\phi + rsin\phi$$
$$z= r\cos\phi + rsin\phi$$
$$\tan\phi = \frac{}{}$$