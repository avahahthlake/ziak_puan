# Input Output and Peripherals

## Memory-Mapped IO (MMIO)

Memory-mapped I/O (MMIO) is a method for a CPU to communicate with peripheral devices by mapping the devices' registers into the same address space used by main memory

## Programmed IO (PMIO)

Programmed I/O (PIO) is a simple data transfer method where the CPU directly controls and manages all data movement between itself and an I/O device


| **Feature**                    | **Memory-Mapped I/O**                   | **Programmed I/O**                  |
| ------------------------------ | --------------------------------------- | ----------------------------------- |
| **Address Space**              | Shares memory address space             | Separate I/O address space          |
| **Instructions Used**          | Normal memory instructions (LOAD/STORE) | Special I/O instructions (IN/OUT)   |
| **Instruction Set Complexity** | Simple (no extra instructions)          | Complex (requires I/O instructions) |
| **Speed**                      | Faster (uses memory operations)         | Slower (extra control steps)        |
| **Hardware Complexity**        | Simpler – unified address decoding      | More complex – separate decoding    |
| **Number of Address Lines**    | No extra lines needed                   | Needs additional I/O control lines  |
| **Flexibility**                | High – full instruction set available   | Limited – only IN/OUT work          |
| **Example Usage**              | Microcontrollers, RISCs                 | Early x86 systems (8085, 8086)      |


## Direct Memory Access (DMA)

It is a technique that allows I/O devices to transfer data directly to/from main memory without involving the CPU for every byte/word.

**DMA is a hardware mechanism that allows peripherals to read/write memory directly, bypassing the CPU, to make high-speed data transfer efficient.**
