# Principle_of_Floating-point_Arithmatic

set x = 0x1.0p1
    y = 0x1.4p2

##
 x + y == (0x1.0p(1 - 2)) + (0x1.4p2)
 x - y == (0x1.0p(1 - 2)) - (0x1.4p2)
 x * y == (0x1.0 * 0x1.4)p(1 + 2)
 x / y == (0x1.0 / 0x1.4)p(1 - 2)
