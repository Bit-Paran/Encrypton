This repository contains a Secure Chat Application developed in Python using the Tkinter library for the user interface and cryptography for all cryptographic operations.

The application implements a Hybrid Cryptography scheme:

User Management: Simple login/signup system. Each user automatically generates an RSA public/private key pair (2048-bit).

Key Exchange: The recipient's RSA Public Key is used to encrypt a unique, symmetric Fernet (AES) key for each message.

Message Encryption: The actual message content is encrypted efficiently using the Fernet (AES) key.

Decryption: Only the intended recipient, possessing the corresponding RSA Private Key, can decrypt the symmetric Fernet key, allowing them to decrypt and read the message.

This project serves as a practical, educational example of how asymmetric (RSA) and symmetric (AES/Fernet) encryption can be combined to form a secure messaging protocol.

Features:

🔒 Secure Login/Signup.

🔑 Automatic RSA Key Pair generation.

💬 Hybrid Encrypted Message Sending/Receiving.

🖼️ Futuristic, full-screen, green-on-black UI with a Matrix-like animation.

💻 Uses standard Python libraries: tkinter, cryptography, os, base64.
