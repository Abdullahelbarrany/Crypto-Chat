
# Crypto-Chat

## Description

SecureChat is a Python-based encrypted chat application that allows two users to securely send and receive messages through a trusted third-party (TTP) server. Inspired by WhatsApp, the app supports multiple encryption algorithms for secure communication. Users can choose from RSA, AES, DES, and ElGamal encryption to encrypt and decrypt messages before transmission.

## Features

**-Two-Client Communication:** Users can send and receive messages via a shared server.

**-Encryption Support:** Choose from RSA, AES, DES, or ElGamal encryption for message security.

**-Tkinter GUI:** User-friendly interface displaying sent messages in black and received messages in blue.

**-Server-Based Architecture:** Uses a central TTP (Trusted Third Party) Server to manage message exchange.
## Tech Stack

**Frontend:** Tkinter-based Python GUI.

**Backend:** Python for message handling and encryption.

**Networking:** Server-client communication model.

**Security:** Four different encryption methods.


## Encryption Algorithms

**1- RSA (Rivest–Shamir–Adleman)**

Uses **public and private key** pairs for encryption.

Encrypts message characters using the formula:

C = M^e mod N

Decryption follows:

M = C^d mod N

**Security:** Hard to break due to large prime factorization.

**2-AES (Advanced Encryption Standard)**

Uses 16-bit key blocks for encryption.

**Rounds of operations:**

    -XOR with key
    -Substitution & shift rows
    -Mix columns
    -Add round key

**Security:** High efficiency, commonly used in modern encryption.

**3-DES (Data Encryption Standard)**

64-bit block cipher with 16 rounds of encryption.

**Steps:**

    -Initial permutation
    -Expansion (EP) & XOR with key
    -S-box substitution
    -Permutation and inverse permutation

**Security:** Weaker than AES but still widely used.

**4-ElGamal Encryption**

Based on the **Diffie-Hellman key exchange**.

Uses **public key cryptography** to encrypt messages.

Each message is encrypted using a **random session key**.

Security: Strong against classical attacks but **vulnerable to quantum computing**.

## How Messages Are Sent & Received

1. User enters a message in the Tkinter GUI.

2. Selects an encryption algorithm (RSA, AES, DES, or ElGamal).

3. Message is encrypted and sent to the server.

4. Server forwards the encrypted message to the recipient.

5. Recipient decrypts the message using the selected algorithm.

6. Decrypted message is displayed in the GUI

<img src="https://github.com/Abdullahelbarrany/Crypto-Chat/blob/main/Screenshot%202023-06-16%20220148.png?raw=true"  align="center" width="300" height="600">
