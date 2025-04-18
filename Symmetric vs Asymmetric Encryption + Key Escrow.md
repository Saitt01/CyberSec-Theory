# 🔐 Symmetric vs Asymmetric Encryption + Key Escrow

## 🧠 Introduzione

La crittografia è fondamentale nella sicurezza informatica per garantire confidenzialità, integrità, autenticazione e non ripudio.  
Esistono due principali categorie di crittografia:
- 🔑 **Crittografia Simmetrica:** utilizza una singola chiave condivisa
- 🔐 **Crittografia Asimmetrica:** utilizza una coppia di chiavi (pubblica e privata)

---

## 🔒 Crittografia Simmetrica

La crittografia simmetrica utilizza **una sola chiave** per cifrare e decifrare i dati. Entrambe le parti devono conoscere e proteggere la stessa chiave.

📌 Esempi:
- AES
- DES, 3DES
- Blowfish, RC4

✅ Vantaggi:
- Molto veloce
- Efficace su grandi quantità di dati

⚠️ Svantaggi:
- Gestione complicata della chiave
- Scalabilità limitata in ambienti complessi

---

## 🔐 Crittografia Asimmetrica

La crittografia asimmetrica utilizza **una coppia di chiavi**: una pubblica per cifrare, una privata per decifrare. Può anche essere usata al contrario per firmare e verificare.

📌 Esempi:
- RSA
- ECC
- DSA
- Diffie-Hellman (per scambio chiavi)

✅ Vantaggi:
- Non serve scambiare la chiave in modo segreto
- Supporta firme digitali e autenticazione

⚠️ Svantaggi:
- Più lenta rispetto alla simmetrica
- Di solito viene usata solo per lo scambio chiavi (es. HTTPS)

---

## 🔄 Confronto

| Caratteristica       | Simmetrica          | Asimmetrica           |
|----------------------|---------------------|------------------------|
| Numero chiavi        | Una condivisa       | Coppia pubblica/privata|
| Velocità             | Veloce              | Più lenta              |
| Scalabilità          | Limitata            | Elevata                |
| Usi comuni           | VPN, file, backup   | HTTPS, firme digitali  |

---

## 📂 Key Escrow

Il key escrow è una pratica in cui una terza parte fidata conserva una copia delle chiavi crittografiche, per usi di emergenza, audit o recupero.

📌 Esempi:
- Recupero dati cifrati aziendali
- Conformità a normative governative

⚠️ Rischi:
- L’escrow deve essere estremamente sicuro
- In caso di compromissione, si rischia un’esposizione totale

---

## 📚 Fonti Consigliate

- CompTIA Security+ Guide  
- OWASP Cryptography Cheat Sheet  
- NIST SP 800-57

---

# ENG VERSION

## 🧠 Introduction

Cryptography is essential in cybersecurity to ensure confidentiality, integrity, authentication, and non-repudiation.  
There are two main types of cryptography:
- 🔑 **Symmetric Encryption:** uses a single shared key
- 🔐 **Asymmetric Encryption:** uses a public/private key pair

---

## 🔒 Symmetric Encryption

Symmetric encryption uses **one single key** to encrypt and decrypt data. Both parties must securely share and manage the same key.

📌 Examples:
- AES
- DES, 3DES
- Blowfish, RC4

✅ Advantages:
- Very fast
- Efficient for large amounts of data

⚠️ Disadvantages:
- Challenging key management
- Poor scalability in large environments

---

## 🔐 Asymmetric Encryption

Asymmetric encryption uses a **key pair**: one public key to encrypt and one private key to decrypt. It can also be used in reverse for signing and verification.

📌 Examples:
- RSA
- ECC
- DSA
- Diffie-Hellman (for key exchange)

✅ Advantages:
- No need for secret key exchange
- Enables digital signatures and authentication

⚠️ Disadvantages:
- Slower than symmetric encryption
- Usually only used for key exchange (e.g., HTTPS)

---

## 🔄 Comparison

| Feature              | Symmetric           | Asymmetric             |
|----------------------|---------------------|------------------------|
| Number of keys       | One shared          | Public/private pair    |
| Speed                | Fast                | Slower                 |
| Scalability          | Low                 | High                   |
| Common use cases     | VPN, file, backups  | HTTPS, digital signatures |

---

## 📂 Key Escrow

Key escrow is the practice of storing cryptographic keys with a trusted third party, for emergency recovery, audits, or regulatory compliance.

📌 Examples:
- Recovery of encrypted corporate data
- Compliance with government regulations

⚠️ Risks:
- Escrow must be extremely secure
- If compromised, all encrypted data may be exposed

---

## 📚 Recommended Sources
  
- CompTIA Security+ Guide  
- OWASP Cryptography Cheat Sheet  
- NIST SP 800-57
