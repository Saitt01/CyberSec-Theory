# 🔐 Data Encryption – Concetti Chiave

## 🧠 Introduzione

La cifratura dei dati è un pilastro della sicurezza informatica. Consiste nel trasformare i dati in un formato illeggibile per chi non possiede la chiave corretta. È utilizzata per proteggere informazioni in vari stati: a riposo, in transito e in uso.

---

## 💾 Encrypting Stored Data

La **cifratura dei dati a riposo** protegge le informazioni memorizzate su dischi, database o dispositivi.

📌 Tecniche comuni:
- Full Disk Encryption (BitLocker, FileVault)
- File-level encryption (GPG, EFS)
- Database encryption

---

## 🗃️ Database Encryption

Protegge i dati archiviati in database da accessi non autorizzati.

📌 Modalità:
- **Transparent Data Encryption (TDE):** cifratura automatica a livello di storage
- **Column-level Encryption:** cifratura selettiva su colonne specifiche
- **Tokenization & Data Masking:** alternative alla cifratura per protezione parziale

---

## 🛰️ Transport Encryption

La **cifratura dei dati in transito** assicura che le informazioni siano protette mentre viaggiano in rete.

📌 Protocolli:
- TLS/SSL (HTTPS, SMTPS, FTPS)
- IPsec (VPN)
- SSH

---

## 🔐 Encryption Algorithms

Gli **algoritmi di cifratura** trasformano dati leggibili in dati cifrati.

📌 Simmetrici:
- AES (standard moderno)
- 3DES, Blowfish

📌 Asimmetrici:
- RSA
- ECC
- ElGamal

---

## 🗝️ Cryptographic Keys

Una **chiave crittografica** è un valore utilizzato dagli algoritmi per cifrare o decifrare i dati.

📌 Tipi:
- Chiave simmetrica: una sola chiave condivisa
- Coppia di chiavi: pubblica + privata (asimmetrica)

---

## 📏 Key Length

La **lunghezza della chiave** influisce sulla sicurezza: più bit = più difficile da violare con brute force.

📌 Esempi:
- AES-128 / AES-256
- RSA-2048 / RSA-4096

🔐 Maggiore lunghezza = maggiore sicurezza ma anche maggiore impatto sulle performance.

---

## 🧠 Key Stretching

Il **key stretching** migliora la forza di password o chiavi deboli aumentandone la complessità computazionale.

📌 Tecniche:
- PBKDF2
- bcrypt
- scrypt
- Argon2

📌 Utilizzato per: protezione di password hashate, derivazione di chiavi da passphrase.

---

## 📚 Fonti Consigliate

- CompTIA Security+ Guide  
- OWASP Cryptography Cheat Sheet  
- NIST SP 800-132  
- Microsoft – TDE & Encryption docs

---

# ENG VERSION

## 🧠 Introduction

Data encryption is a foundational component of cybersecurity. It transforms readable data into unreadable format without the correct key. Encryption protects data at rest, in transit, and in use.

---

## 💾 Encrypting Stored Data

**Encrypting data at rest** protects information stored on disks, databases, or devices.

📌 Common techniques:
- Full Disk Encryption (BitLocker, FileVault)
- File-level encryption (GPG, EFS)
- Database encryption

---

## 🗃️ Database Encryption

Protects sensitive information stored in databases from unauthorized access.

📌 Modes:
- **Transparent Data Encryption (TDE):** automatic encryption at storage level
- **Column-level Encryption:** targeted encryption on specific fields
- **Tokenization & Data Masking:** alternatives for partial protection

---

## 🛰️ Transport Encryption

**Encrypting data in transit** secures information while it travels across networks.

📌 Protocols:
- TLS/SSL (HTTPS, SMTPS, FTPS)
- IPsec (VPN)
- SSH

---

## 🔐 Encryption Algorithms

**Encryption algorithms** convert plaintext into ciphertext.

📌 Symmetric:
- AES (modern standard)
- 3DES, Blowfish

📌 Asymmetric:
- RSA
- ECC
- ElGamal

---

## 🗝️ Cryptographic Keys

A **cryptographic key** is a value used by an algorithm to encrypt or decrypt data.

📌 Types:
- Symmetric key: one shared key
- Asymmetric pair: public + private keys

---

## 📏 Key Length

**Key length** impacts security: more bits = harder to break with brute force.

📌 Examples:
- AES-128 / AES-256
- RSA-2048 / RSA-4096

🔐 Longer key = stronger encryption, but higher performance cost.

---

## 🧠 Key Stretching

**Key stretching** strengthens weak passwords or keys by making them computationally expensive to crack.

📌 Techniques:
- PBKDF2
- bcrypt
- scrypt
- Argon2

📌 Used for: hashing password storage, deriving keys from passphrases.

---

## 📚 Recommended Sources

- CompTIA Security+ Guide  
- OWASP Cryptography Cheat Sheet  
- NIST SP 800-132  
- Microsoft – TDE & Encryption docs
