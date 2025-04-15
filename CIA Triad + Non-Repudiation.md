# 🔐 CIA Triad + Non-Repudiation

## 🧠 Introduzione
La **CIA Triad** rappresenta i tre principi fondamentali della sicurezza delle informazioni. Qualsiasi misura di sicurezza deve essere progettata per proteggere almeno uno di questi aspetti.

---

## 🔒 C - Confidentiality (Riservatezza)
Garantisce che **solo le persone autorizzate** possano accedere ai dati.

📌 Esempi:
- Crittografia (AES, RSA)
- Controlli di accesso (ACL, RBAC)
- Autenticazione utente

🛡️ **Obiettivo:** Impedire l'accesso non autorizzato a dati sensibili.

---

## 🧬 I - Integrity (Integrità)
Assicura che i dati non vengano **alterati o modificati** senza autorizzazione.

📌 Esempi:
- Hashing (SHA-256, MD5 con HMAC)
- Controllo versione
- Firma digitale

🛡️ **Obiettivo:** Garantire che le informazioni siano accurate e affidabili.

---

## ⚙️ A - Availability (Disponibilità)
I dati devono essere **accessibili quando necessario**, da utenti autorizzati.

📌 Esempi:
- Backup e ridondanza
- Sistemi di failover
- Protezione da attacchi DoS/DDoS

🛡️ **Obiettivo:** Evitare interruzioni nel servizio o nella disponibilità delle risorse.

---

## 🧾 Non-Repudiation (Non Ripudio)
Garantisce che una parte **non possa negare** di aver eseguito un'azione (come inviare un messaggio o effettuare una transazione).

📌 Esempi:
- Firma digitale con chiave privata
- Log immutabili
- Timestamps certificati

🛡️ **Obiettivo:** Fornire **prove inconfutabili** che una determinata azione è stata compiuta da una specifica entità.

---

## 📌 Riepilogo
| Principio | Obiettivo | Tecnologie Chiave |
|----------|-----------|-------------------|
| Confidentiality | Evitare accessi non autorizzati | Crittografia, autenticazione |
| Integrity | Prevenire modifiche ai dati | Hashing, firme digitali |
| Availability | Assicurare accesso continuo | Backup, protezione DoS |
| Non-Repudiation | Impedire il disconoscimento | Firme digitali, logging |

---

## 📚 Fonti Consigliate
- CompTIA Security+ Official Guide
- OWASP Foundations
- NIST SP 800-53


# ENG VERSION:
# 🔐 CIA Triad + Non-Repudiation

## 🧠 Introduction
The **CIA Triad** represents the three core principles of information security. Every security measure should be designed to protect at least one of these aspects.

---

## 🔒 C - Confidentiality
Ensures that **only authorized individuals** can access data.

📌 Examples:
- Encryption (AES, RSA)
- Access control mechanisms (ACL, RBAC)
- User authentication

🛡️ **Goal:** Prevent unauthorized access to sensitive data.

---

## 🧬 I - Integrity
Ensures that data is not **altered or tampered with** without authorization.

📌 Examples:
- Hashing (SHA-256, MD5 with HMAC)
- Version control
- Digital signatures

🛡️ **Goal:** Ensure data is accurate and trustworthy.

---

## ⚙️ A - Availability
Ensures that data is **accessible when needed** by authorized users.

📌 Examples:
- Backups and redundancy
- Failover systems
- Protection against DoS/DDoS attacks

🛡️ **Goal:** Avoid disruptions to service or resource availability.

---

## 🧾 Non-Repudiation
Ensures that an entity **cannot deny** having performed a specific action (e.g., sending a message or making a transaction).

📌 Examples:
- Digital signature with private key
- Immutable logging
- Certified timestamps

🛡️ **Goal:** Provide **irrefutable proof** that a specific action was carried out by a specific party.

---

## 📌 Summary
| Principle         | Goal                             | Key Technologies             |
|------------------|----------------------------------|------------------------------|
| Confidentiality   | Prevent unauthorized access       | Encryption, authentication   |
| Integrity         | Prevent unauthorized modifications | Hashing, digital signatures  |
| Availability      | Ensure continuous access          | Backup, DoS protection       |
| Non-Repudiation   | Prevent denial of actions         | Digital signatures, logging  |

---


## 📚 Recommended Sources
- CompTIA Security+ Official Guide  
- OWASP Foundations  
- NIST SP 800-53
