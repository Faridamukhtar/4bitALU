# 4bitALU
This is a logisim simulation of a simple arithmetic unit (ALU) that is capable of adding, subtracting and getting remainder of two signed magnitude numbers, and displays the result of the operation using three 7-segments. Some flags are used as well to show the status of the output.
# Description
The arithmetic unit takes two 4-bits signed inputs, 𝐴 and 𝐵, (for example +7= 0111, -2= 1010) and an additional 2bits input called Mode of Operation, which informs the arithmetic unit which function to perform on 𝐴 and 𝐵, the Output C is a 7-bits signed inputs (C is composed of 6-bits for the value and 1-bit for the sign):
1. (00) Addition 𝐶=𝐴 + 𝐵
2. (01) Subtraction 𝐶=𝐴 − 𝐵
3. (11) Remainder: C = A % B
# Flags
### Sign Flag:
The sign flag indicates if the result is negative. The flag is set to 1 if the result is negative and 0
otherwise (i.e., the output is zero or positive number). A % B, has the same sign as A.
### Zero Flag:
The zero flag indicates if the result is zero. The flag is set to 1 if the result is zero and 0 otherwise.
### Div by Zero Flag:
The divide by zero flag indicates if we divide by zero. The flag is set to 1 if B operand (the second
operand) equals zero in reminder operation and 0 otherwise.
