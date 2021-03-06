# Principle_of_Floating-point_Arithmatic

## example of principle

 **x = 0x1.0p1; y = 0x1.4p2**
```
  x + y == (0x1.0p(1 - 2)) + (0x1.4p2)
  x - y == (0x1.0p(1 - 2)) - (0x1.4p2)
  x * y == (0x1.0 * 0x1.4)p(1 + 2)
  x / y == (0x1.0 / 0x1.4)p(1 - 2)
```

## steps description

**addition:**
  - 1 check and process zero
  - 2 equalize exponents
  - 3 add signed significands
  - 4 normalize and round result

**subtraction:**
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

## special numbers
```
  Not_a_Number == 0.0 / 0.0
  Positive_Infinity == 1.0 / 0.0
  Negative_Inginity == -1.0 / 0.0
```

## rounding policy
1. round toward nearest
2. round toward positive_infinity
3. round toward negative_infinity
4. round toward zero
