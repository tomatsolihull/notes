- To store decimal numbers in a [[Binary]] format, it is necessary to convert them to a standardised format. One of the options for doing this is floating point numbers.
- There are many different [[Standard]]s and formats for storing floating point numbers

# [[IEEE]] [754](https://ieeexplore.ieee.org/search/searchresult.jsp?queryText=754%20Standard%20for%20Floating-Point%20Arithmetic&highlight=true&returnType=SEARCH&matchPubs=true&refinements=ContentType:Standards&returnFacets=ALL&sortType=newest)
- Numbers are stored as a fixed length with an exponent and a mantissa element.  
- **Half** = 16 bits = binary16
- **Single** = 32 bits = binary32
- **Double** = 64 bits = binary64
- **Quad** = 128 bits = binary128
- **Octuple** = 256 bits = binary256

# Converting [[Binary]] to Singles
$\Large{111110100.011111_{\text{Base 2}} = 01000011111111010001111100000000_{\text{IEEE 754 binary32}}}$
## 1. Normalising
The first step is **normalising**.
This is moving the decimal point as far to the left as possible, similar to scientific notation.

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