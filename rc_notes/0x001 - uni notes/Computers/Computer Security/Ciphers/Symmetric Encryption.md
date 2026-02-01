---
author: rc
class: note
tags:
description:
source:
related:
date created: 2026-01-31T16:02:00
last update: 2026-02-01T15:26:30
aliases:
---
Symmetric encryption uses the same key for encryption and decryption. This requires both parties to know the key. Thus the key needs to be shared in a secure way.

Symmetric encryption are fast and small (hardware/software).

Symmetric encryption ciphers are usually block ciphers or Symmetric block ciphers. They work on a fixed data length (16 bytes). Encrypting more than the block size requires multiple runs. Encrypting less than the block size requires padding


- Examples
	- AES
	- DES
	- 3DES
	- RC4


# Advanced Encryption Standard (AES)

AES has a block size of 16 bytes (128 bits) of input plaintext. It also outputs 16 bytes of ciphertext.

It can have one of 3 key sizes
- AES-128: 16 bytes (10 rounds)
- AES-192: 24 bytes (12 rounds)
- AES-256: 32 bytes (14 rounds)

The round key remains the same size of 16 bytes.

## Rounds



# (DES)