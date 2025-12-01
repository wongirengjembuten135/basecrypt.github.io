# [BaseCrypt](https://basecrypt.github.io)
![Argon2id](https://img.shields.io/badge/Argon2id-15%20iterations-blue)
![HKDF-SHA3-256](https://img.shields.io/badge/HKDF--SHA3--256-derive%20keys-green)
![XChaCha20-Poly1305](https://img.shields.io/badge/XChaCha20--Poly1305-encrypt-orange)
![HMAC-SHA3-512](https://img.shields.io/badge/HMAC--SHA3--512-integrity-red)

![](https://github.com/BaseCrypt/basecrypt.github.io/releases/download/1.1/base.png)

[BaseCrypt](https://basecrypt.github.io) — **A small, fully client-side tool for strongly protected text encryption.**  

Cloud sucks, servers suck, everything sucks — so everything happens on yourұ device, no bytes go anywhere.

## What It Does
Type text → set a passphrase → get a link like `#note=verylonggarbage`.  
Drop it anywhere: thread, PM, chat.  
Recipient opens, enters passphrase — text pops up. Done.  
No data leaves your device. Fully client-side.  

Works as long as github.io is up and you have the HTML file.
By the way you can also just download a small HTML (3 MB)  

[![Download HTML](https://img.shields.io/badge/Download-HTML-blue?style=for-the-badge)](https://github.com/basecrypt/basecrypt.github.io/releases/download/1.3/basecrypt.html)  
SHA256: ``5f121b41fa8a699e0290d457a55404453f20a7624abc4ca9ca119dff01669c57``

## How It Works
- **Create** — type → encrypt → output (...encrypt)   
- **Open** — open from URL (...decrypt)  
- **Read** — paste URL or data manually (...decrypt)

## Cryptography
- Argon2id (15 iterations, 64 MB memory, 4 threads) → master key  
- HKDF-SHA3-256 → encryption key + MAC key  
- XChaCha20-Poly1305  
- HMAC-SHA3-512

## Limitations
- Links never expire. Anyone with the link can try the passphrase.  
- Max size: **30,000 chars**.

## Support
This is fully open-source, contained entirely in a small HTML file, free, and always publicly available.
