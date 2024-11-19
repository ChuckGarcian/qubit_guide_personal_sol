
# Converting 1 + eipsi to polar

\newcommand{\ep}{e^{i\psi}}
\newcommand{\eph}{e^{i\frac{\psi}{2}}}
\newcommand{\ephm}{e^{-i\frac{\psi}{2}}}
\newcommand{\ph}{\frac{\psi}{2}}
**Claim 1:** Given the complex number $z = 1 + e^{i\theta}$, we claim:
$$
z = 1 + e^{i\theta} = 2 \eph \cos\ph 
$$
**Proof:**
$$1 + \ep$$
$$
\Rightarrow \text{<1 = $e^{i \cdot 0}$>}
$$
$$
e^{i \cdot 0} + \ep
$$
$$
\Rightarrow \text{<$0 \equiv \frac{\psi}{2} - \frac{\psi}{2}, \psi \equiv \frac{\psi}{2} + \frac{\psi}{2}$>}
$$
$$
e^{i(\ph - \ph)} + e^{i(\ph)}
$$
$$
\Rightarrow
$$
$$
\eph\ephm + \eph\eph
$$
$$
\Rightarrow
$$
$$
\eph \left(\ephm + \eph \right)
$$
$$
\Rightarrow \text{< Euler's identity: $e^{i\theta} = \cos\theta + i\sin\theta$>}
$$
$$
\eph \left[ (\cos\ph + i\sin\ph) + (\cos\ph - i\sin\ph)\right]
$$
$$
\Rightarrow
$$
$$
\eph \left( 2\cos\ph \right)
$$
$$
\Rightarrow
$$
$$
2 \eph \cos\ph 
$$
$\blacksquare$


-----


**Claim 1.5:** Given the complex number $z = 1 - e^{i\theta}$, we claim:
$$
z = 1 - e^{i\theta} =  -2i\cdot\eph\cdot\sin\ph 
$$
**Proof:**
$$1 - \ep$$
$$
\Rightarrow \text{<1 = $e^{i \cdot 0}$>}
$$
$$
e^{i \cdot 0} + \ep
$$
$$
\Rightarrow \text{<$0 \equiv \frac{\psi}{2} - \frac{\psi}{2}, \psi \equiv \frac{\psi}{2} + \frac{\psi}{2}$>}
$$
$$
e^{i(\frac{\psi}{2} - \frac{\psi}{2})} - e^{i(\frac{\psi}{2} + \frac{\psi}{2})}
$$
$$
\Rightarrow
$$
$$
\eph\ephm - \eph\eph
$$
$$
\Rightarrow
$$
$$
\eph \left(\ephm - \eph \right)
$$
$$
\Rightarrow \text{< Euler's identity: $e^{i\theta} = \cos\theta + i\sin\theta$>}
$$
$$
\eph \left[ \left( \cos\ph - i\sin\ph \right) - \left(\cos\ph - i\sin\ph \right)\right]
$$
$$
\Rightarrow
$$
$$
\eph \left[ \cos\ph - i\sin\ph - \cos\ph + i\sin\ph\right]
$$
$$
\Rightarrow
$$
$$
\eph \left( -2i\sin\ph \right)
$$
$$
\Rightarrow
$$
$$
-2i\cdot\eph\cdot\sin\ph 
$$
$\blacksquare$