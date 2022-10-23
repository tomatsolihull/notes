Binary is a Base-2 [[Positional Numeral Systems]] and is the way computers fundamentally store data at the lowest level.

# Bit
- Lowest and most basic way of representing information in computing
- Represent the electrical signals that are being manipulated and stored by a computer
- Either 1 or 0  (on or off)

# Nibble
A group of four bits

# Sextet
Group of six bits

# Byte
Group of eight bits

# Octet
More specific term for a group of eight bits

# Hextet
Group of sixteen bits

# Conversions
## [[Denary (Decimal)]] to/from [[Binary]]
$\Large{123_{10} = 01111011_{2}}$
$$
\begin{array}{|r|r|r|r|r|r|r|r|}
\hline
128=2^7 & 64=2^6 & 32=2^5 & 16=2^4 & 8=2^3 & 4=2^2 & 2=2^1 & 1=2^0 \\
\hline
0 & 1 & 1 & 1 & 1 & 0 & 1 & 1 \\
\hline
\end{array}
$$
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

### Decimal Points
$\Large{123_{10} = 01100.1100_{2}}$

$$\textbf{Before Decimal = 12}$$
$$
\begin{array}{|r|r|r|r|}
\hline
16=2^4 & 8=2^3 & 4=2^2 & 2=2^1 & 1=2^0 \\
\hline
0 & 1 & 1 & 0 & 0 \\
\hline
\end{array}
$$
$$\textbf{After Decimal = 0.75}$$
$$
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