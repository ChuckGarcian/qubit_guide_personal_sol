# Notes

\newcommand{\OO}{\ket{0}\bra{0}}
\newcommand{\ol}{\ket{0}\bra{1}}
\newcommand{\lo}{\ket{1}\bra{0}}
\newcommand{\LL}{\ket{1}\bra{1}}

Suppose we have a one dimensional universe represented by an array whose entries contain the state of each cells (i.e. one or zero). We can define a high order operator which describes the evolution of the universe also refered to as the update function $uf(\ket{bbb})$ where $\ket{bbb}$ is the current state. 


## High Order Definition of update function - No unitrary (no dense linear algebra)

Suppose we define the uf in the following high order definition


**Bit 0 Rule**

$$
\begin{aligned}
    \ket{00b} &\mapsto \ket{00b} \\
    *\ket{01b} &\mapsto \ket{01\bar b} \\
    \ket{10b} &\mapsto \ket{10b} \\
    *\ket{11b} &\mapsto \ket{11\bar b} \\
\end{aligned}
$$

**Bit 1 Rule**

$$
\begin{aligned}
    \ket{0b0} &\mapsto \ket{0b0} \\
    * \ket{0b1} &\mapsto \ket{0 \bar b1} \\
    * \ket{1b0} &\mapsto \ket{1 \bar b 0} \\    
    \ket{1b1} &\mapsto \ket{1b1} \\
\end{aligned}
$$

**Bit 2 Rule**

$$
\begin{aligned}
    \ket{b00} &\mapsto \ket{b00} \\
    \ket{b01} &\mapsto \ket{b01} \\
    *\ket{b10} &\mapsto \ket{\bar b10} \\
    *\ket{b11} &\mapsto \ket{\bar b11} \\
\end{aligned}
$$

## Low Order - Dense linear algebra based definition with unitrary

**Bit 0 Rule**

$$
\begin{matrix}
\OO \cdot  \OO \cdot I \\
\OO \cdot \LL \cdot A \\
\LL \cdot \OO \cdot I \\
\LL \cdot \LL \cdot A \\
\end{matrix}
$$

**Bit 0 Rule**

$$
\begin{matrix}
\OO \cdot I \cdot \OO \\
\OO \cdot A \cdot \LL \\
\LL \cdot A \cdot \OO \\
\LL \cdot I \cdot \LL
\end{matrix}
$$

**Bit 2 Rule**

$$
\begin{matrix}
I \cdot \OO \cdot \OO \\
I \cdot \OO \cdot \LL \\
A \cdot \LL \cdot \OO \\ 
A \cdot \LL \cdot \LL \\
\end{matrix}
$$

## Generalization

In general given a bit vector $\ket{a_0 a_1 b}$ where b is to be updated, we can describe the update with a boolean function $f: B^3\mapsto B^1$. From the above example we could define the boolean function as $x_{3} = f (\vec{s}) = (x_{0}\land x_{1})\lor x_3$ where 3 is the bit we are updating (b). So in general we need a boolean function for each bit.  

bit 0: $x_{0} = f (\vec{s}) =  x_1 \land \neg x_0$

bit 1: $x_{1} = f (\vec{s}) = \neg x_1 \lor x_0$

bit 2: $x_{2} = f (\vec{s}) = (x_{0}\land x_{1})\lor x_3$

------

**Crux:** I think the crux of this is that given a high level definition of a CA we need a systematic way to derive a unitary matrix which carries out the computation elegantly. 

## Example: CCNOT. High vs Low order definitions

$$
\begin {matrix}
    \ket{00b} &\mapsto \ket{00b} \\
    \ket{00b} &\mapsto \ket{01b} \\
    \ket{10b} &\mapsto \ket{10b} \\
    *\ket{11b} &\mapsto \ket{11\bar b} \\
\end {matrix}
\longrightarrow 
\begin{matrix}
\OO \cdot  \OO \cdot I \\
\OO \cdot \LL \cdot I \\
\LL \cdot \OO \cdot I \\
\LL \cdot \LL \cdot X \\
\end{matrix}
$$

Therefore:    

So rule $f_0$ is a linear operator, defined as:

$f_0 = \OO \cdot  \OO \cdot I +
\OO \cdot \LL \cdot I +
\LL \cdot \OO \cdot I +
\LL \cdot \LL \cdot X$, 

Hence $f_0$ implements ccnot

We could then have a rule for the other 2 bits $f_1, f_2$

The evolution of the entire system is therefore the set of operators associated with each qubit $F$


Therefore: $$F = \{ f_0, f_1, f_2 \}$$

The matrix representation of the entire eovlution is therefore given as: 

$$F = f_0 + f_1 + f_2$$

## Crux: My formalism

CA: 
**Input:** 3 element tuple $(F, )$

## Laws of Quantum based logic

## Laws of Chuckian Algebra


