Base 16 ([[zk/Positional Numeral System]])

One base 16 digit (0-F) represents 4 bits

# Denoting Hex
- `0xABCD`
- `#ABCD`
- `%ABCD`
- `\xABCD`
- `0hABCD`
- $ABCD_{16}$
-  $ABCD_{hex}$

# Converting [[zk/Denary (Decimal)]] to [[zk/Hexadecimal]]


$\Large{123_{10} = \text{7B}_{16}}$
$$
\begin{array}{|r|r|r|r|}
\hline
4096=16^3 & 256=16^2 & 16=16^1 & 1=16^0 \\
\hline
0 & 0 & 123\div16=7.6875 & 123\mod16=11\\
\hline
\end{array}
$$
$$
\lfloor7.6875\rfloor = 7
$$
$$
11 = \text{B}
$$


$\Large{541_{10} = \text{21D}_{16}}$
$$
\begin{array}{|r|r|r|r|}
\hline
4096=16^3 & 256=16^2 & 16=16^1 & 1=16^0 \\
\hline
0 & 541\div256=2.1133 & 541\mod256=29 & 29\mod16=13\\
 &                   & 29\div16=1.8125  & \\

\hline
\end{array}
$$
$$
\lfloor2.1133\rfloor = 2
$$
$$
\lfloor1.8125\rfloor = 1
$$
$$
13 = \text{D}
$$


#  Lookup Table
| Base 10 | Base 16 | Base 2 |
| -       | -       | -      |
| 0       | 0       | 0000   |
| 1       | 1       | 0001   |
| 2       | 2       | 0010   |
| 3       | 3       | 0011   |
| 4       | 4       | 0100   |
| 5       | 5       | 0101   |
| 6       | 6       | 0110   |
| 7       | 7       | 0111   |
| 8       | 8       | 1000   |
| 9       | 9       | 1001   |
| 10      | **A**   | 1010   |
| 11      | **B**   | 1011   |
| 12      | **C**   | 1100   |
| 11      | **D**   | 1101   |
| 14      | **E**   | 1110   |
| 15      | **F**   | 1111   |