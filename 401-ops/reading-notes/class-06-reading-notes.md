# Class 06 Reading Assignment

## Data File Encryption

- Applying the CIA triad to Your Enterprise File Transfer ([article](https://www.jscape.com/blog/implementing-the-cia-triad-when-transferring-files-through-the-internet))
- What are MD5, SHA-1, and SHA-256 Hahes, and How Do I Check Them? ([article](https://www.howtogeek.com/67241/htg-explains-what-are-md5-sha-1-hashes-and-how-do-i-check-them/))

## Questions

1. **You have been made responsible for the company’s file server. How would you preserve the three elements of the CIA triad?**
   - _Confidentiality:_ Enforce strong encryption protocols for data in transit and at rest, and apply strict authentication and authorization checks to control access.
   - _Integrity:_ Utilize hash functions to detect alterations, and implement digital signatures for non-repudiation and integrity verification during file transfers.
   - _Availability:_ Set up high availability systems to ensure server uptime and redundancy, and protect against service disruptions through consistent monitoring and robust network infrastructure.
2. **Explain how hashing verifies data integrity using non-technical terms.**
   - Hashing is like taking the fingerprint of a file, word, or sentence. There is only one fingerprint that matches that file and when you share this fingerprint, others can use it to verify by they have an unchanged and uncorrupted of the file by taking their own fingerprint of it and comparing the two. If they match, then they have a perfect and unaltered copy of the original!
3. **How is hashing and encryption different?**
   - Hashing is a one-way process, you cannot de-hash something. However, you can 'crack' a hash by brute forcing (or using a rainbow table) to try and recreate the hash.
   - Encryption, on the other hand, is reversible. It does require knowing the exact parameters that were used to encrypt the data and also knowing the key that was used.

