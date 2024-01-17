# Class 06 - Data File Encryption and Hashing

## Encryption

**Encryption** is the act of transforming plaintext into ciphertext.

- Ensures data _confidentiality_ (of the CIA triad)

**Encryption** uses a cipher, or a mathematical algorithm, to transform readable plaintext into unreadable ciphertext.

### Ciphertext

- **Ciphertext** is the altered form of a plaintext message, so as to be unreadable for anyone except the intended recipients.
  - Ciphertext is something that has been turned into a "secret" through encryption.
  - Ensures data _confidentiality._
- **Plaintext** is human readable. **Ciphertext** looks like gibberish.

### Decryption

- **Decryption** is the reverse process of encryption.
  - Converts a ciphertext message back into plaintext.
  - Uses a cryptographic algorithm and the appropriate key that was used in the original encryption of the message.

### Hashing

- **Hashing** is a process that generates a unique has value for a given data.
  - Can target a file or a string.
    - Hashing strings is a common way passwords are "stored".
  - Hashing is a one-way process. Cracking a hash involves trying to replicate the hash value
- A **hash value** is a unique value that corresponds to the content of the file.
  - Message Digest 5 (MD5)
  - Secure Hashing Algorithm 1 (SHA-1)
  - SHA-2
  - NTLM
  - LANMAN

<center><img src="https://codefellows.github.io/ops-401-cybersecurity-guide/curriculum/class-06/slides/assets/05_03.png" width=500/></center>

## Data Transimission Security

### Data States

- **Data at Rest**
  - The data is in some sort of persistent storage media.
- **Data in Transmit** (or Data in Motion)
  - The data is being transmitted over a network.
    - Examples:
      - Website Traffic
      - Remote access traffic
      - Data being synchronized between cloud repositories.
- **Data in Use** (or data in processing)
  - Data is present but in volatile memory.
    - RAM
    - CPU registers and caches

### Data in Motion

- **Data Confidentiality**

  - PII, trade secrets, customer lists, key employee salaries, marketing strategies, source codes, etc. Ensuring it doesn't fall into the wrong hands.

- **Data Integrity**

  - Data remains unchanged.
  - Or if it is changed, you are made aware.

- **Data Source Authenticity**
  - Data actually came from who it claims to have come from.
  - Man in the Middle Attacks target modifying data source.

## Data Transmission Protocols

### TLS

- **Transport Layer Security (TLS)**

  - Typically used with the HTTP application (referred to as _HTTPS_ or _HTTP Secure_)
  - TLS can also be used to secure other application protocols and as a VPN (virtual private networking) solution.
  - Versions include:
    - 1.3
    - 1.2
    - 1.1
    - 1.0
  - These are all still in active use.

- **Downgrade Attack**
  - A type of _Man-in-the-middle_ attack that tries to force the use of a weak cipher suite and SSL/TLS version.
  - TLS 1.3 is impervious to downgrade attack.

### FTP vs SFTP

- **File Transfer Protocol (FTP)** facilitates the transfer of files between hosts.
  - Uses TCP/IP
  - Connection established on **TCP port 21**
  - Username/password crednetials are sent in plaintext.
    - VERY INSECURE
-**Secure File Transfer Protocol (SFTP)** facilitates the *secure* transfer of files between hosts.
  - It does this by utilizing SSH with encrypted credentials.
  - Connects through **TCP port 22**.

