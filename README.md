# Image-Encryption-Decryption-using-AES
## Overview

This project implements an AES-based image encryption and decryption system using Python. The project demonstrates the core working principles of the Advanced Encryption Standard (AES) algorithm by manually implementing AES transformations such as SubBytes, ShiftRows, MixColumns, AddRoundKey, and their corresponding inverse operations for decryption.

The system encrypts image files into encrypted binary `.enc` format and restores the original image during decryption using the same secret key.

---

## Features

- AES-inspired manual implementation
- 128-bit secret key generation
- Image encryption and decryption
- Galois Field multiplication
- SubBytes transformation using AES S-Box
- ShiftRows operation
- MixColumns transformation
- AddRoundKey operation
- Inverse AES operations for decryption
- Encrypted output stored as `.enc` binary file
- Exact image restoration after decryption

---

## Technologies Used

- Python
- NumPy
- Pillow (PIL)
- Secrets
---

## AES Operations Implemented

### Encryption

1. SubBytes
2. ShiftRows
3. MixColumns
4. AddRoundKey
5. Random Key Generation
6. Padding

### Decryption

1. AddRoundKey
2. Inverse MixColumns
3. Inverse ShiftRows
4. Inverse SubBytes
5. Entered the Decryption key

---

## Project Workflow

## Input Image

![Input Image](Sample/input_image.png)

---

##

![Encrypted Text](Sample/encyrpted.png)

---

## Decrypted Image

![Decrypted Image](Sample/decrypted_image.png)

### Encryption Process

Input Image  
→ Convert Image to Binary Byte Data  
→ Divide into 16-byte Blocks  
→ AES Encryption Operations  
→ Encrypted `.enc` File

### Decryption Process

Encrypted `.enc` File  
→ AES Decryption Operations  
→ Remove Padding  
→ Restore Original Image

---



## Installation

Install required libraries using pip:

```bash
pip install numpy pillow secrets
