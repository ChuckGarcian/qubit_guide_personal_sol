# 2.14.2 Change of basis

**Answer:**

$$\ket\psi = \frac{3}{5}\ket0 + \frac{4}{5}\ket1$$

We can rewrite $\psi$ in normal vector notation:

$$
\ket\psi =
\frac{3}{5} 
\begin{bmatrix}
1 \\
0
\end{bmatrix} +
\frac{4}{5} 
\begin{bmatrix}
0 \\
1
\end{bmatrix}
$$

$$
\ket\psi
=
\begin{bmatrix}
\frac{3}{5} \\
\frac{4}{5} 
\end{bmatrix}$$

We can think of that vector as the coordate vector for $\ket\psi$ in the standard basis. We want to find the coordinate vector $\ket\psi$ in the hadamard basis. That is we solve for $\alpha$ and $\beta$:
$$
\ket\psi
=
\begin{bmatrix}
\frac{3}{5} \\
\frac{4}{5} 
\end{bmatrix}
= \alpha \ket{+} + \beta \ket{-}
$$

$$
\begin{bmatrix}
\frac{3}{5} \\
\frac{4}{5} 
\end{bmatrix} =
\frac{\alpha}{\sqrt2}
\begin{bmatrix}
1 \\
1
\end{bmatrix} +
\frac{\beta}{\sqrt2} 
\begin{bmatrix}
1 \\
-1
\end{bmatrix}
$$


$$
\begin{bmatrix}
\frac{3\sqrt2}{5} \\
\frac{4\sqrt2}{5} 
\end{bmatrix} =
\alpha
\begin{bmatrix}
1 \\
1
\end{bmatrix} +
\beta
\begin{bmatrix}
1 \\
-1
\end{bmatrix}
$$


$$
\begin{bmatrix}
\frac{3\sqrt2}{5} \\
\frac{4\sqrt2}{5} 
\end{bmatrix} =
\begin{bmatrix}
\alpha + \beta \\
\alpha -\beta
\end{bmatrix}
$$

From the matrix equation:
$$\frac{3\sqrt{2}}{5} = \alpha + \beta$$
$$\frac{4\sqrt{2}}{5} = \alpha - \beta$$
Adding the equations:
$$2\alpha = \frac{7\sqrt{2}}{5}$$
$$\alpha = \frac{7\sqrt{2}}{10}$$
Subtracting the equations:
$$2\beta = -\frac{\sqrt{2}}{5}$$
$$\beta = -\frac{\sqrt{2}}{10}$$
Therefore:
$$\alpha = \frac{7\sqrt{2}}{10} \approx 0.99$$
$$\beta = -\frac{\sqrt{2}}{10} \approx -0.14$$