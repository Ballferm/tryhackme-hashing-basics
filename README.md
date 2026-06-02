# tryhackme-hashing-basics
TryHackMe Hashing Basics lab covering cryptographic hashing, password security, rainbow tables, Hashcat, HMACs, and integrity verification.
# TryHackMe - Hashing Basics

## Overview

This room introduced the fundamentals of cryptographic hashing and its role in cybersecurity.

The lab explored how hash functions are used for:

- Data integrity verification
- Password storage
- Password cracking
- Authentication mechanisms
- Message authentication

The room also demonstrated the security risks of weak password storage methods and the importance of salting passwords before hashing.

---

## Objectives

- Understand how hash functions work
- Learn the differences between MD5, SHA1 and SHA256
- Explore password hashing concepts
- Understand rainbow table attacks
- Learn how salts improve password security
- Identify different hash formats
- Practice basic hash cracking techniques
- Understand integrity checking and HMACs

---

## Key Concepts Learned

### Hash Functions

A hash function converts data of any size into a fixed-size output.

Important properties include:

- Deterministic output
- One-way operation
- Fixed output length
- Avalanche effect

A single-bit change in the input produces a completely different hash.

---

### Password Storage

Instead of storing plaintext passwords, systems should store password hashes.

Benefits:

- Reduced exposure during breaches
- Difficult for attackers to recover passwords directly

---

### Password Salting

A salt is a unique random value added to a password before hashing.

Benefits:

- Prevents identical passwords from generating identical hashes
- Protects against rainbow table attacks
- Improves password security significantly

---

### Rainbow Tables

Rainbow tables are precomputed databases of password hashes.

Attackers use them to quickly reverse weak unsalted hashes.

Adding unique salts makes rainbow tables ineffective.

---

### Password Cracking

The room introduced password cracking using:

- Online hash lookup databases
- Wordlists
- Hashcat

This demonstrated why weak passwords remain vulnerable even when hashed.

---

### Integrity Verification

Hashes can verify that files have not been altered.

If a downloaded file produces the same hash as the publisher's hash, the file integrity can be trusted.

---

### HMACs

HMAC (Hash-based Message Authentication Code) combines:

- A secret key
- A cryptographic hash function

HMACs help verify:

- Authenticity
- Integrity

of transmitted data.

---

## Tools Used

- TryHackMe AttackBox
- Hashcat
- SHA256SUM
- MD5SUM
- SHA1SUM
- CrackStation
- Hashes.com

---

## Practical Activities Completed

- Generated MD5, SHA1 and SHA256 hashes
- Compared hash outputs for similar files
- Identified hash algorithms
- Investigated password storage methods
- Explored rainbow table attacks
- Cracked password hashes
- Verified file integrity using SHA256 hashes
- Studied HMAC authentication workflows

---

## Skills Developed

- Cryptographic hashing fundamentals
- Password security concepts
- Hash identification
- Hash cracking methodology
- File integrity validation
- Security analysis mindset

---

## Screenshots

Screenshots documenting the exercises are stored in the `/screenshots` directory.

---

## Reflection

This room strengthened my understanding of how hashing supports authentication, integrity verification, and password security.

One of the most valuable lessons was seeing how weak hashing practices and unsalted passwords can be vulnerable to rainbow table attacks, while modern techniques such as salting and stronger algorithms significantly improve security.

This knowledge is directly relevant to SOC analysis, digital forensics, incident response, and defensive cybersecurity operations.

---

## Completion Status

Completed Successfully ✅

Platform: TryHackMe

Room: Hashing Basics
