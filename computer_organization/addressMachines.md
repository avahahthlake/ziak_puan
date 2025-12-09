# 1-Address machine 📢
  * This uses what's called the accumulator architecture
  * While the second operand and the result are implicitly stored in a
  dedicated CPU register -> ***accumulator***
  * Hardware is simple (as it only manages a single explicit operand)
  * It has very short instruction length.
  * For complex programs, code becomes more.
  * They require frequent memory access to load operands and store result.
  This can hinder performance.

# 1-1/2 Address machine 🕧
  * One operand is explicitly a memory address.
  * Another operand is explicitly named register.
  * It is different from a pure 2 Address machine, in the sense that
   *this architecture balances the flexibility of memory access* with the speed
   of register operations.
  * Example... ADD R1, A ..... {add the content of memory location A to R1}
  * It has more flexibility and power.
  * Instructions are longer than a 1-Address machine, because fields for
  opcode, register and memory addresses are required.
  * Memory access is less frequent per computation.
  * Code is more compact *due to fewer lines of code* than a 1-address machine instruction.

# Load 🔃, Shift 🤫, Branch 🪹 instructions (formal description).
### Load 🔃
```format
LD Rd, Address

where Rd = destination register
Address = Memory address
```

The load instruction copies the value stored at a specified memory
address into the destination register.

### Shift 🤫
```format
SHL Rd, Rn, s ; shift left // bit shifted out of MSB
SHR Rd, Rn, s ; shift right // bit shifted out of LSB
SAR Rd, Rn, s ; arithmetic shift right // bit shifted out of LSB

where Rd = destination register
      Rn = source register
      s = shift amount
```

### Branch 🪹
```format
BR target // unconditional
BR꜀꜀ target // conditional

where target = branch target address
```

