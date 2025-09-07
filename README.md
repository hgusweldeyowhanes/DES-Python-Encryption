# DES Encryption and Decryption in Python

A Python implementation of the **Data Encryption Standard (DES)** algorithm for encrypting and decrypting text messages.
This project demonstrates the process of DES, including 
--> key generation, 
--> initial and final permutations, 
--> expansion, 
--> S-box substitutions, 
--> XOR operations.

## Features

- Encrypt and decrypt messages using the DES algorithm.
- Supports **PKCS5 padding** for messages not multiple of 8 bytes.
- Implements all 16 rounds of DES with proper key scheduling.
- Fully written in Python without external dependencies.
- Educational and practical implementation for learning cryptography concepts.


## Installation
--> pip install numpy
--> pip install cryptography

  ## Algorithm Details
The implementation follows the standard DES steps:
  1, Initial Permutation (IP) on the plaintext.
  2, Splitting the plaintext into left and right halves.
  3, 16 Rounds of DES:
  4, Expansion (E) of right half.
  5, XOR with the round key.  
  6, S-box substitution.  
  7, Permutation (P) of the result.  
  8, XOR with left half and swapping.  
  9, Final Permutation (FP) after the 16 rounds.  
  10, Key schedule uses PC1, PC2, and SHIFT tables to generate 16 round keys.  
  11, Supports PKCS5 padding to handle messages that are not multiples of 8 bytes.
    
 ## Example 
  Enter the message to be encrypted:
  HELLO WORLD
  Enter a key of 8 length:
  mysecret
  Encrypted Ciphertext is : '...'
  Decrypted plaintext is  : HELLO WORLD
 

