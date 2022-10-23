#networking
# Internet Protocol version 6


## Addressing
- No subnet masks, only uses [[Slash Notation]]
- Broken up into eight 'hextets' (16-bits each) and written in [[Hexadecimal]]
- 128 bits long

### Compression Rules
`2001:0db8:85a3:0000:0000:8a2e:0370:7334`

1. The longest and leftmost set of continuous zeros is replaced with `::`
   `ef82:0000:0000:0000:1a12:0000:0234:1b12`
   becomes `ef82::1a12:0000:0234:1b12`
2. Leading zeros in hextets can be removed, but one number must remain (even if it is a zero)
   `ef82::1a12:0000:0234:1b12`
   becomes `ef82::1a12:0:234:1b12`