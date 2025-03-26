![image](https://github.com/user-attachments/assets/ecdf51fa-2dc1-4fbd-b28d-077e3aaa7a2b)


The challenge takes a 64-character input and performs a transformation using ROT13 and bitwise operations before checking it against a predefined value.

Key Steps:

Input Handling: Reads user input (expected to be 64 characters).

ROT13-like Transformation: Each character is shifted by 13 and masked with 0x7F.

Reversal: The transformed string is reversed (except for the first and last characters).

Bitwise XOR: The final string is XORed with 0x03.

Comparison: The result is checked against "C@qpl==Bppl@<=pG<>@l>@Blsp<@l@AArqmGr=B@A>q@@B=GEsmC@ArBmAGlA=@q" to verify correctness.

Solution Approach:

To retrieve the flag, reverse the process:

XOR the target string with 0x03 to recover the intermediate state.

Reverse the transformation order to reconstruct the original rot array.

Apply inverse ROT13 to get the original input.

So; the correct input is: e615b75a4d563ac971466e05641d7aed556b62fcb460b6027f126bff411bfe63


![image](https://github.com/user-attachments/assets/db733f1b-74af-44ea-b82f-89948bc8c7fb)


AND GG.
