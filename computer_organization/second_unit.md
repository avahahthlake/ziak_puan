# Ways of representing numbers in a computer system.🔢

## Unsigned representation 🫩

* Uses all bits to represent non-negative integers.
* Range of n bits 0 to 2ⁿ-1

## Signed-number representation

### Sign magnitude representation

* MSB = sign bit(0 -> +, 1 -> -)
* Remaining bits store the magnitude
* Example (8-bit)
  * +5 = 00000101
  * -5 = 10000101
* Drawbacks
  * Two representations of zero
  * arithmetic computations are complicated since you have to handle
    the sign bit separately.

### One's complement representation

* Negative numbers are obtained by complementing every bit.
  (1 -> 0, 0 -> 1)
* Example... +5 -> 00000101, -5 -> 11111010
* Addition requires end-around carry which complicates it.

### Two's complement representation

* Negative number = (bitwise complement) + 1
* Used in modern computers.
* Example ... +5 = 00000101, -5 = 11111011
* It solves the problem of "multiple zeros"
* It does simple addition and subtraction using binary adders.
* For n bits, its range is -2ⁿ⁻¹-1 to 2ⁿ⁻¹-1

Two's complement is the most appropriate representation because...

* unique zero
* same hardware for addition and subtraction
* automatic overflow handling
* simpler and faster hardware design
