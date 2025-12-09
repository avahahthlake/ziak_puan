# Concpetual view of memory cell 🧑‍🔬

* Fundamental unit of digital storage. An electronic circuit storing single bit (0 or 1) that can be set, reset and read; acting like tiny switch or capacitor that holds its state until changed. These building blocks are arranged in order such that they form the computer memory.
* One-bit storage - only holds one binary digit (0 or 1)
* Bistable state - two stable states 1 & 0
* Addressable - organised in the form of arrays with unique address.
* Read/Write operations - stored bit read and written over

## There are two types of memory cells. 🕑

* Static RAM (SRAM) -> This kind of memory cell uses flip-flops (transistors) to store date, holding it as long as power is available.

* Dynamic RAM (DRAM) -> This uses capacitors and transistors, the capacitor holds charge (1) or no charge(0) but needs refreshing.

### Access time ⌛

Access time is the total time delay between a request for a piece of data or instruction by the CPU (or another system component) and the "moment" that data is retrieved and available for use.

### Bandwidth 🤕

Bandwidth is the maximum data transfer capacity of a network connection, in a given amount of time.

## Direct mapped and associated mapped cache 🗺

A cache is a temporary storage location that holds copies of frequently used data to speed up access time.

* Direct mapped cache -> This is a cache design where each block from main memory can only go into one specific, predetermined line in the cache. Determined by the memory address.
* Associative mapped cache -> This is a cache mechanism that allows a main memory block to be stored in any cache line.

## Paging 📃

Paging is the process of moving parts of a program called pages from hard-disks to RAM. The main purpose of paging in memory management, is to break a program into smaller fixed-size blocks called *pages*.

### Working of paging 👹

* A process requests memory
* The processor allocates one or more page frames to the process.
* The processor maps the process' logical pages to the physical page frames.
* When a program runs, it's pages are loaded into any available frames in the physical memory.

## Translation lookaside buffer 🤔 [TLB]

* TLB is a hardware cache that speeds-up memory access by storing recent translations of virtual memory address to physical memory address.
* It reduces the time taken to access memory by essentially looking up for the physical memory address first.
