# [[Denary (Decimal)]] $\leftrightarrows$ [[Binary]]
$123_{10} = 01111011_{2}$

| 128 $2^7$  | 64 $2^6$ | 32 $2^5$ | 16 $2^4$ | 8 $2^3$ | 4 $2^2$ | 2 $2^1$ | 1 $2^0$ |
| - | - | - | - | - | - | - | - |
| 0 | 1 | 1 | 1 | 1 | 0 | 1 | 1 |

$$
(0 \times 128) +
(1 \times 64) +
(1 \times 32) +
(1 \times 16) +
(1 \times 8) +
(0 \times 4) +
(1 \times 2) +
(1 \times 1)
= 123
$$

## Decimal Points
$123_{10} = 01100.1100_{2}$

$$
\textbf{Before Decimal = 12 }

\begin{array}{|r|r|r|r|}
\hline
16=2^4 & 8=2^3 & 4=2^2 & 2=2^1 & 1=2^0 \\
\hline
0 & 1 & 1 & 0 & 0\\
\hline
\end{array}
$$

$$
\textbf{After Decimal = 0.75 }
\begin{array}{|r|r|r|}
\hline
0.5=2^{-1} & 0.25=2^{-2} & 0.125=2^{-3} &0.0625=2^{-4} \\
\hline
1 & 1 & 0 & 0 \\
\hline
\end{array}
$$

$8 + 4 = 12$
$0.5 + 0.25 = 0.75$

$12 + 0.75 = 12.75$

---

# [[Binary]] $\to$ 32-Bit [[Floating Point Numbers]]
$111110100.011111_{2} = 01000011111111010001111100000000_{\text{IEEE 754}}$

## 1. Normalising
The first step is **normalising**. This is moving the decimal point as far to the left as possible, similar to scientific notation.

$111110100.011111 \times 2^0 \to 1.11110100011111 \times 2^8$
Where the new exponent $8$ is because we've moved the decimal point eight places to the left.

## 2. Exponent
The second step is calculating the **exponent part** of the number.
To do so, we must add 127 to our exponent and convert the result to binary.

$8 + 127 = 135$
$135 \to 10000111$

## 3. Formatting
A 32-bit number must be 32 bits long.

The **sign** is a single bit that indicates whether the number is positive or negative.
0 = positive, 1 = negative.

The **exponent*** is eight bits long.

The **mantissa*** is twenty three bits long. It is also known as the fraction portion.
It must be [padded with zeros](https://github.com/tomatsolihull/scripts-etc/blob/master/mantissa23padding.js) at the end to make it 23 bits long.

$$
\begin{array}{r|r|l}
\text{Sign} & \text{Exponent} & \text{Mantissa} \\
\hline
0 & 10000111 & 111110100011111\textit{00000000}
\end{array}
$$

---

# [[Denary (Decimal)]] $\to$ [[Octal & Hexadecimal]]

## Octal (Base 8 )
- Digits 1-7

$31072_{8} = 12858_{10}$
| 4096 $8^4$ | 512 $8^3$ | 64 $8^2$ | 8 $8^1$ | 1 $8^0$ |
| - | - | - | - | - |
| 3 | 1 | 0 | 7 | 2 |

$$
(3 \times 4096) +
(1 \times 512) +
(0 \times 64) +
(7 \times 8) +
(2 \times 1)
= 12858
$$