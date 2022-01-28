# Bit Manipulation

Every Number is represented in decimal format in day to day life but in computer it is being converted to binary(0,1)

Types of Numbers and resp. powers:

1. Decimal-10(0-9)
2. Binary-2(0,1)
3. HexaDeximal-16(0-9,a-f)
4. Octa-8(0-7)


## Convertion

### Convertion from Decimal to Any Other

Divide by power of convertion number(2, 8, 16) until became < 0, keep track of remainders, the reverse order of remainders is the answer

### Convertion from Any other to Decimal

Keep adding the multiplication of bit (starting from LSB) with 2 raised to the power bit index's.
For example: for 1010 in bin.
1*(2^3) + 0*(2^2) + 1*(2^1) + 0*(2^0) = 10(in decimal);

## Operators

### AND (&) operator

& operators give 1(for all 1) and 0(for any 0)

example: 
if a=5, b=6 then a&b = 4
a=5 -> 101
b=6 -> 110
a&b -> 100(4)

### OR (|) operator
| operators give 1(for any 1) and 0(for all 0)

example:
if a=5, b=6 then a|b = 7
a=5 -> 101
b=6 -> 110
a|b -> 111(7)

### XOR (^) operator

^ gives 0(even 1) and 1(odd 1).
example:
if a=7, b=5
a=7 -> 111
b=5 -> 101
a^b -> 010(2)

### Negation (~) operator

~ operator flips the bit i.e., 0->1, 1->0

### Right Shift (>>) operator

'>>' will shift the bit by one postion to the right side

example: if a = 6
a>>1 means 110>>1 = 011(3)
a>>2 means 110>>2 = 001(1)

'>>' operator divides the number by 2^b where b is number of times to right shift
if a=10, a>>2 = a/(2^2) = 10/4 = 2
a=10 -> 1010 >>2 = 0010(2)

### Left Shift (<<) operator

'<<' will shift the bit by one position to the left side ahead.

exmaples: if a= 6;
a<<1 means (110<<1) = 1100(12)

<< operator multifly the number by 2^b
