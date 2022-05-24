# Principle_of_Floating-point_Arithmatic
#
**example:**

 x = 0x1.0p1; y = 0x1.4p2
```
  x + y == (0x1.0p(1 - 2)) + (0x1.4p2)
  x - y == (0x1.0p(1 - 2)) - (0x1.4p2)
  x * y == (0x1.0 * 0x1.4)p(1 + 2)
  x / y == (0x1.0 / 0x1.4)p(1 - 2)
```
#
## steps description
#
**addition**
  - 1 check zero
  - 2 equalize exponents
  - 3 add signed significands
  - 4 normalize and round result

**suntraction**
  - 1 check zero and flip sign of minuend
  - 2 equalize exponents
  - 3 add signed significands
  - 4 normalize and round result
#
