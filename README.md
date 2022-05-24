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
**addition:**
  - 1 check and process zero
  - 2 equalize exponents
  - 3 add signed significands
  - 4 normalize and round result

**suntraction:**
  - 1 check and process zero
  - 2 flip sign of minuend
  - 3 equalize exponents
  - 4 add signed significands
  - 5 normalize and round result

**multiplication**
  - 1 check and process zero
  - 2 get sum of exponents
  - 3 multiply signed significands
  - 4 normalize and round result

**division**
  - 1 check and process zero
  - 2 get difference of exponents
  - 3 divide signed dignificands
  - 4 normalize and round result
#
