# 🎭 Deception & Disruption nella Cybersecurity

## 🧠 Introduzione

Nel contesto della sicurezza informatica, i concetti di **Deception** (inganno) e **Disruption** (interruzione) rappresentano due approcci **proattivi** per contrastare gli attaccanti.  
A differenza delle difese tradizionali (come firewall e antivirus), queste tecniche mirano a **interferire direttamente con l'attività dell’attaccante**.

---

## 🎭 Deception (Inganno)

La **deception** consiste nell'ingannare l'attaccante inducendolo a interagire con risorse **false ma realistiche**, così da rallentarlo e raccogliere informazioni utili sul suo comportamento.

### 📌 Esempi di tecniche di deception:
- **Honeypot:** Sistema fittizio progettato per essere attaccato.
- **Honeynet:** Intera rete di honeypot interconnessi, che simula un'infrastruttura reale.
- **Honeytoken:** File o credenziale-trappola inserita nei sistemi (es. `admin:123456` in un database esca).
- **Honeyfile:** Documento-trappola che genera un alert se aperto o copiato (es. "passwords.xlsx").
- **Decoy Networks:** Ambienti virtuali che imitano reti e servizi reali per sviare l’attaccante.

🛡️ **Obiettivo:** Confondere l'attaccante, rallentare la compromissione e raccogliere indicatori di compromissione (IOC).

---

## 💥 Disruption (Interruzione)

La **disruption** mira a **interferire direttamente con le attività dell'attaccante**, bloccando o degradando il suo accesso una volta rilevato.

### 📌 Esempi di tecniche di disruption:
- Disconnessione automatica da VPN
- Reset immediato di password o token compromessi
- Isolamento della macchina colpita dalla rete
- Blocco temporaneo di IP sospetti
- Interruzione di una sessione remota in corso

🛡️ **Obiettivo:** Ridurre i danni, fermare la lateral movement e guadagnare tempo per rispondere all'incidente.

---

## 🔄 Deception vs Disruption

| Strategia   | Scopo principale            | Esempi                                  |
|-------------|-----------------------------|------------------------------------------|
| Deception   | Ingannare e osservare       | Honeypots, honeyfiles, decoy networks    |
| Disruption  | Interrompere l’attacco      | Isolamento host, blocco accessi, reset   |

---

## 📚 Fonti Consigliate
- MITRE Engage (ex MITRE Shield)  
- NIST Cybersecurity Framework  
- Cyber Deception Playbook (MITRE)  
- TryHackMe – Deception Techniques


# ENG VERSION

# 🎭 Deception & Disruption in Cybersecurity

## 🧠 Introduction

In cybersecurity, **Deception** and **Disruption** are **proactive defense techniques** used to interfere with and mislead attackers.  
Unlike traditional defenses (e.g., firewalls, antivirus), these strategies are designed to **confuse or actively block threat actors** in real time.

---

## 🎭 Deception

**Deception** involves tricking attackers into interacting with **fake but realistic resources**, slowing their progress and exposing their behavior.

### 📌 Examples of deception techniques:
- **Honeypot:** Fake system intentionally exposed to attackers.
- **Honeynet:** A simulated network made of multiple interconnected honeypots.
- **Honeytoken:** Trap credential or file placed in critical systems (e.g., `admin:123456`).
- **Honeyfile:** Trap file that triggers alerts when opened (e.g., "passwords.xlsx").
- **Decoy Networks:** Simulated environments that mimic real services and networks.

🛡️ **Goal:** Confuse the attacker, delay progression, and collect indicators of compromise (IOCs).

---

## 💥 Disruption

**Disruption** aims to **actively interfere with an attack** after it has been detected, to prevent further damage.

### 📌 Examples of disruption techniques:
- Auto-disconnect from VPN sessions
- Forced password/token reset
- Isolating the compromised host
- Blocking suspicious IPs
- Killing an active shell or remote session

🛡️ **Goal:** Limit damage, prevent lateral movement, and buy time to respond effectively.

---

## 🔄 Deception vs Disruption

| Strategy     | Main Purpose               | Examples                                |
|--------------|----------------------------|------------------------------------------|
| Deception    | Mislead and monitor        | Honeypots, honeyfiles, decoy networks    |
| Disruption   | Block or interrupt attacks | Host isolation, credential resets        |

---


## 📚 Recommended Sources
- MITRE Engage (formerly MITRE Shield)  
- NIST Cybersecurity Framework  
- MITRE Cyber Deception Playbook  
- TryHackMe – Deception Rooms

