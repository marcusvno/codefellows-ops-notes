# Class 05 - Encryption Basics

## Data States

- **Data at Rest**
  - The data is in some sort of *persistent* storage media.
- **Data in transit (or data in motion)**
  - The data is being *transmitted* over a network.
  - Examples:
    - Website Traffic
    - Remote access traffic
    - Data being synchronized between cloud repositories
- **Data in use (data in processing)**
  - When an application or file is accessed, data in use is placed in RAM.

## Encryption

**Encryption** is the act of transforming *plaintext* into *ciphertext*.
  - Ensures data *confidentiality*.

## Ciphertext

## Hashing

Hashing is a process that generates a unique hash value for a given data.
    - Can target a file or a string.

A hash value is a unique value that corresponds to the content of the file. Checking the hash after receiving a file to the original hash allows you to see if the file has been modified in transit.

- Common hashes algorithms:
  - Message Digest 5 (MD5)
  - Secure Hashing Algorithm 1 (SHA-1)
  - SHA-2
  - NTLM
  - LANMAN