# 🗃File organization

File organization deals with how data is ***stored efficiently*** for
***efficient access*** moving from data-fields->records->files 

To do such feats, we can use methods like
  * sequential(linear)
  * direct/hash(fast lookup via hashing)
  * indexed-sequential

🚽 So, the main purpose of file-organization is to speed up file-accessing

🚽 file-organization is the backbone of file systems like NTFS, FAT32 etc.


# 📈Data hierarchy

  * Bit/Byte -> This is the smallest unit of data
  * Field/Attribute -> A single piece of data like name, id, salary, etc.
  * Record -> A collection of related fields. (📈database-vibe)
  * File -> A collection of related records...

# 📁File Attribute

File Attributes are metadata that describe the details of a file...

like...
  * its name
  * size
  * location
  * creation time/date 
  * modified
  * last-access
  ...

# 💬Text files vs 🌓binary file

The difference between a text file and a binary file lies on their encoding
and interpretation of data


| text-files | binary-files |
| -------------- | --------------- |
| human readable | machine readable |
| character encoding | application-specific encoding |
| line endings | diverse data types and no specific line endings |


Examples of text files are...
  * Source code files like .py, .c, .java, etc...
  * Normal text files like .txt, .docx, .md itself here

Examples of binary files are...
  * Executable program files that end with .exe, .dmg, etc
  * Photo files like .jpg, .png
  * Audio files like .wav, .flac, .mpg, etc...


# Common 📁File organization methods🧑‍🏭
  1. sequential -> records stored one after another ***in order***
  2. heap -> records places wherever space is available
  3. direct -> using hash functions to calculate storage address for random and quick accessing, fast but chance of collisions
  4. 
