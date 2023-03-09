## Pre-Lab preparation

1. Write characteristic equations and complete truth tables for D, JK, T flip-flops where `q(n)` represents main output value before the clock edge and `q(n+1)` represents output value after the clock edge.   

![Characteristic equations](eq_flip_flops.png)
<!--
https://editor.codecogs.com/
\begin{align*}
    q_{n+1}^D =&~D \\
    q_{n+1}^{JK} =& \\
    q_{n+1}^T =& \\
\end{align*}
-->

   **D-type FF**
   | **clk** | **d** | **q(n)** | **q(n+1)** | **Comments** |
   | :-: | :-: | :-: | :-: | :-- |
   | ![rising](eq_uparrow.png) | 0 | 0 | 0 | `q(n+1)` has the same level as `d` |
   | ![rising](eq_uparrow.png) | 0 | 1 | 0 | `q(n+1)` has the same level as `d` |
   | ![rising](eq_uparrow.png) | 1 | 0 | 1 | `q(n+1)` has the same level as `d` |
   | ![rising](eq_uparrow.png) | 1 | 1 | 1 | `q(n+1)` has the same level as `d` |

   **JK-type FF**
   | **clk** | **j** | **k** | **q(n)** | **q(n+1)** | **Comments** |
   | :-: | :-: | :-: | :-: | :-: | :-- |
   | ![rising](eq_uparrow.png) | 0 | 0 | 0 | 0 | Output did not change |
   | ![rising](eq_uparrow.png) | 0 | 0 | 1 | 1 | Output did not change |
   | ![rising](eq_uparrow.png) | 0 | 1 | 0 | 0 | Reset |
   | ![rising](eq_uparrow.png) | 0 | 1 | 1 | 0 | Reset |
   | ![rising](eq_uparrow.png) | 1 | 0 | 0 | 1 | Set |
   | ![rising](eq_uparrow.png) | 1 | 0 | 1 | 1 | Set |
   | ![rising](eq_uparrow.png) | 1 | 1 | 0 | 1 | Toogle |
   | ![rising](eq_uparrow.png) | 1 | 1 | 1 | 0 | Toogle |

   **T-type FF**
   | **clk** | **t** | **q(n)** | **q(n+1)** | **Comments** |
   | :-: | :-: | :-: | :-: | :-- |
   | ![rising](eq_uparrow.png) | 0 | 0 | 0 | Output did not change |
   | ![rising](eq_uparrow.png) | 0 | 1 | 1 | Output did not change |
   | ![rising](eq_uparrow.png) | 1 | 0 | 1 | Toogle |
   | ![rising](eq_uparrow.png) | 1 | 1 | 0 | Toogle |

<a name="part1"></a>