# Decimal Numbers
- 0
- 1
- 2
- 3
- 4
- 5
- 6
- 7
- 8
- 9
- Decimal numbers are 10 digit.
- Decimal numbers is used for human counting.
- Base 10.
# Binary Numbers
- 0
- 1
- Binary numbers are 2 digits.
- Binary numbers is used for computer understanding.
- Base 2.
# Decimal vs Binary
- Decimal and Binary always diff 2 digits. 
```c++
int d0 = 0;
int d1 = 1;
int d2 = 2;
int d3 = 3;
int d4 = 4;
int d5 = 5;
int d6 = 6;
int d7 = 7;
int d8 = 8;
int d9 = 9;
```

```c++
int b0 = 0;
int b1 = 1;
int b2 = 10;
int b3 = 11;
int b4 = 100;
int b5 = 101;
int b6 = 110;
int b7 = 111;
int b8 = 1000;
int b9 = 1001;
```


---

# Octal Numbers
- 0
- 1 
- 2
- 3
- 4
- 5
- 6
- 7
- Octal Numbers are 8 digits.
- Base 8.
# Hexadecimal Numbers
- 0
- 1
- 2
- 3
- 4
- 5
- 6
- 7
- 8
- 9
- A
- B
- C
- D
- E
- F
- Hexadecimal Numbers are 16 digits.
- Base 16.

|Decimal|Binary|Octal|Hexadeciaml|
|----|---|----|----|
|0|0000|000|0|
|1|0001|001|1|
|2|0010|002|2|
|3|0011|003|3|
|4|0100|004|4|
|5|0101|005|5|
|6|0110|006|6|
|7|0111|007|7|
|8|1000|010|8|
|9|1001|011|9|
|10|1010|012|A|
|11|1011|013|B|
|12|1100|014|C|
|13|1101|015|D|
|14|1110|016|E|
|15|1111|017|F|


---
# Just for fun it (convert decimal to decimal)
$$
\begin{flalign}
&=273\\
&=200 + 70 + 3 \\
&=2*100 + 7*10 + 3*1 \\
&=2*10^2 + 7*10^1 + 3*10^0\\
&=2*b^2 + 7*b^1 + 3*b^0\\
\end{flalign}
$$
##### ==Convert Binary,Octal,Hexadecimal To Decimal== -01
$$
\begin{flalign}
&=1101\\
&=1*b^3+ 1*b^2 + 0*b^1 + 1*b^0\\
&=1*2^3+ 1*2^2 + 0*2^1 + 1*2^0\\
&=1*8 + 1*4 + 0*2 + 1*1\\
&=8+4+0+1\\
&=13
\end{flalign}
$$

# Just for fun it(convert  decimal to decimal)
$$
\begin{flalign}
&=273\\
&=10)\frac{273}{3}(27 \\
&=10)\frac{27}{7}(2 \\
&=10)\frac{2}{2}(0 \\
&=b)\frac{2}{2}(0 \\
&reminder=273(MSB-LSB)\\
\end{flalign}
$$

##### ==Convert Deciaml To Binary, Octal, Hexadecimal== -02

$$
\begin{flalign}
&=13\\
&=2)\frac{13}{1}(6 \\
&=2)\frac{6}{0}(3 \\
&=2)\frac{3}{1}(1 \\
&=2)\frac{1}{1}(0 \\
&=1101(MSB-LSB)\\
\end{flalign}
$$
#####  ==Convert One to Another Number Systems== -03
- Step-01: first convert into decimal.
- Step-01: then convert into desired number system
---
