# Notes

Suppose we have a one dimensional universe represented by an array whose entries contain the state of each cells (i.e. one or zero). We can define a high order operator which describes the evolution of the universe also refered to as the update function $uf(\ket{bbb})$ where $\ket{bbb}$ is the current state. 

## High Order Definition of update function

Suppose we define the uf in the following high order definition

$$
\begin{aligned}
    \ket{0b0} &\mapsto \ket{0b0} \\
    * \ket{1b0} &\mapsto \ket{1 \bar b0} \\
    * \ket{0b1} &\mapsto \ket{0 \bar b1} \\
    \ket{1b1} &\mapsto \ket{1b1} \\
\end{aligned}
$$

$$
\begin{aligned}
    \ket{0b0} &\mapsto \ket{0b0} \\
    \ket{0b1} &\mapsto \ket{0b1} \\
    \ket{1b0} &\mapsto \ket{0b1} \\
    \ket{1b1} &\mapsto \ket{1b1} \\
\end{aligned}
$$

$$
\begin{aligned}
    \ket{1b0} &\mapsto \ket{1b0} \\
    \ket{1b0} &\mapsto \ket{1b0} \\
    \ket{1b1} &\mapsto \ket{1b1} \\
\end{aligned}
$$

## Low Order

\newcommand{\OO}{\ket{0}\bra{0}}
\newcommand{\ol}{\ket{0}\bra{1}}
\newcommand{\lo}{\ket{1}\bra{0}}
\newcommand{\LL}{\ket{1}\bra{1}}

$$
\begin{matrix}
\OO I \OO \\
\LL I \OO \\
\OO I \LL \\
\LL A \LL
\end{matrix}
$$

$$
\begin{matrix}
\OO \cdot  \OO \cdot I \\
\OO \LL A \\
\LL \OO I \\
\LL \LL A \\
\end{matrix}
$$

$$
\begin{matrix}
I \cdot \OO \cdot \OO \\
I \OO \LL  \\
I \LL \OO \\ 
A \LL \LL \\
\end{matrix}
$$
