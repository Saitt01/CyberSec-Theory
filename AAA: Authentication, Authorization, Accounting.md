# 🔐 AAA: Authentication, Authorization, Accounting

## 🧠 Introduzione
Il modello **AAA** (Authentication, Authorization, Accounting) è un framework fondamentale nella sicurezza informatica, utilizzato per **controllare l'accesso** e **monitorare le attività degli utenti** in sistemi informatici e reti.

---

## 🔑 Authentication (Autenticazione)
È il processo con cui un sistema verifica **l'identità di un utente o entità**.

📌 Esempi:
- Login con username + password
- Autenticazione a più fattori (MFA)
- Certificati digitali
- Token hardware/software

🛡️ **Obiettivo:** Verificare *chi sei*.

---

## 🧾 Authorization (Autorizzazione)
Una volta autenticato, il sistema determina **a cosa puoi accedere** e con quali permessi.

📌 Esempi:
- Accesso solo in lettura a una cartella
- Permesso di eseguire comandi specifici
- Politiche RBAC (Role-Based Access Control)

🛡️ **Obiettivo:** Definire *cosa puoi fare*.

---

## 📊 Accounting (Rendicontazione / Tracciamento)
Tiene traccia di **cosa fa un utente nel sistema**: login, logout, accesso a risorse, modifiche effettuate.

📌 Esempi:
- Log di sistema
- Monitoraggio di sessioni VPN
- Audit trail per accesso ai file

🛡️ **Obiettivo:** Registrare *quando, dove e cosa è stato fatto*.

---

## 📌 Riepilogo
| Componente     | Descrizione                     | Esempi                          |
|----------------|----------------------------------|----------------------------------|
| Authentication | Verifica dell'identità           | Password, MFA, certificati       |
| Authorization  | Controllo degli accessi          | ACL, RBAC, policy                |
| Accounting     | Monitoraggio delle attività      | Log, auditing, session tracking |

---

## 📚 Fonti Consigliate
- CompTIA Security+ Guide  
- RFC 2865 (RADIUS)  
- NIST Identity and Access Management



# ENG VERSION

# 🔐 AAA: Authentication, Authorization, Accounting

## 🧠 Introduction
The **AAA model** (Authentication, Authorization, Accounting) is a foundational framework in cybersecurity used to **control access** and **monitor user activity** in systems and networks.

---

## 🔑 Authentication
The process through which a system verifies the **identity of a user or entity**.

📌 Examples:
- Login with username + password
- Multi-Factor Authentication (MFA)
- Digital certificates
- Hardware/software tokens

🛡️ **Goal:** Verify *who you are*.

---

## 🧾 Authorization
After authentication, the system defines **what resources you can access** and what actions you are allowed to perform.

📌 Examples:
- Read-only access to a folder
- Permissions to execute specific commands
- RBAC policies (Role-Based Access Control)

🛡️ **Goal:** Define *what you can do*.

---

## 📊 Accounting
Tracks **what the user does** in the system: logins, logouts, resource access, file modifications, etc.

📌 Examples:
- System logs
- VPN session tracking
- File access audit trails

🛡️ **Goal:** Record *when, where, and what was done*.

---

## 📌 Summary
| Component       | Description                    | Examples                        |
|----------------|--------------------------------|---------------------------------|
| Authentication | Identity verification           | Password, MFA, certificates     |
| Authorization  | Access control                  | ACLs, RBAC, policies            |
| Accounting     | Activity tracking               | Logs, auditing, session logs    |

---

## 📚 Recommended Sources
- CompTIA Security+ Guide  
- RFC 2865 (RADIUS)  
- NIST Identity and Access Management

