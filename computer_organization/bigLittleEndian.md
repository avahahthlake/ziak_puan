# Big 🦣 and Little 🐁 Endian.

Big Endian and Little Endian refers to the byte order when storing data in the main memory.

* ***Big Endian*** stores data's MSB(most significant bit) first.
* ***Little Endian*** stores data's LSB(least significant bit) first.

Example of Big Endian

| 0x100 | 0x101 | 0x102 | 0x103 |
|   -   |   -   |   -   |   -   |
|   01  |   23  |   45  |   67  |

Example of Little Endian

| 0x100 | 0x101 | 0x102 | 0x103 |
|   -   |   -   |   -   |   -   |
|   67  |   45  |   23  |   01  |