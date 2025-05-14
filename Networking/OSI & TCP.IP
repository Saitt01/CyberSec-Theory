# 🧱 Modelli di Rete – OSI & TCP/IP

## 🧩 Introduzione

Due modelli fondamentali spiegano come i dati viaggiano da un dispositivo all’altro in una rete:  
- Il **modello OSI (Open Systems Interconnection)**  
- Il **modello TCP/IP (Transmission Control Protocol / Internet Protocol)**

Sono strumenti di riferimento importanti per la **cybersecurity**, soprattutto durante:
- l’analisi del traffico,
- il debugging delle comunicazioni,
- i penetration test,
- la comprensione di attacchi di rete (es. sniffing, spoofing, hijacking...).

Studiare entrambi i modelli è **fondamentale** per avere una visione chiara di come funziona la comunicazione in rete.

---

## 🌐 Modello OSI – 7 Livelli

### 🎯 Obiettivo
Il modello OSI è stato progettato per standardizzare il modo in cui **sistemi e tecnologie diverse comunicano tra loro**, tramite una struttura a livelli.  
Ogni livello svolge un compito ben definito e comunica solo con i livelli immediatamente sopra e sotto.

---

### 📚 I 7 Livelli OSI (dall’alto verso il basso)

| Livello | Nome                 | Funzione                                                                 |
|--------:|----------------------|--------------------------------------------------------------------------|
| 7       | **Applicazione**     | Interfaccia diretta con l’utente. Gestisce input/output dei dati.       |
| 6       | **Presentazione**    | Traduce, cripta o decripta i dati in un formato comprensibile per l’app.|
| 5       | **Sessione**         | Gestisce le connessioni (sessioni) tra dispositivi.                     |
| 4       | **Trasporto**        | Controlla il flusso e l’integrità dei dati tra host (es. TCP).          |
| 3       | **Rete**             | Indirizzamento logico e routing dei pacchetti (es. IP).                 |
| 2       | **Collegamento Dati**| Gestisce la trasmissione senza errori nella rete locale (es. MAC).      |
| 1       | **Fisico**           | Trasmette i bit fisicamente (cavi, onde, segnali elettrici).            |

---

### 🧠 Dettagli importanti

- I livelli **1-2** gestiscono la parte fisica e locale della rete.
- I livelli **3-4** sono orientati al **trasporto dei dati** tra host.
- I livelli **5-7** gestiscono l’interazione con l’utente e l’applicazione.
- Ogni pacchetto attraversa tutti i livelli **dal 7 al 1** in invio, e **dall’1 al 7** in ricezione.
- Ogni livello aggiunge un **header** con informazioni di controllo → **incapsulamento**.

---

## 🌐 Modello TCP/IP – 4 Livelli

### 🎯 Obiettivo
Il modello TCP/IP è quello realmente usato su Internet.  
È anche chiamato **Internet Protocol Suite** e unisce più funzioni rispetto all’OSI, in soli **4 livelli**.

---

### 📚 I 4 Livelli TCP/IP

| Livello | Nome           | Funzione                                                                 |
|--------:|----------------|--------------------------------------------------------------------------|
| 4       | **Applicazione**| Protocollo usato da programmi come browser, email, DNS, ecc.             |
| 3       | **Trasporto**   | Gestione delle connessioni (es. TCP affidabile, UDP veloce ma non sicuro)|
| 2       | **Internet**    | Indirizzamento IP e routing dei pacchetti attraverso più reti            |
| 1       | **Link**        | Invio e ricezione fisica dei dati sulla rete (Ethernet, WiFi, ecc.)      |

---

## 🔁 PDU – Unità di Dati per Livello

Ogni livello gestisce i dati in un formato chiamato **PDU (Protocol Data Unit)**.

| Livello OSI       | Livello TCP/IP | Nome PDU         |
|-------------------|----------------|------------------|
| Application (7-5) | Application     | **Dati**         |
| Transport (4)     | Transport       | **Segmento**     |
| Network (3)       | Internet        | **Pacchetto**    |
| Data-Link (2)     | Link            | **Frame**        |
| Physical (1)      | Link            | **Bit**          |

---

## ⚔️ Confronto tra OSI e TCP/IP

| Modello OSI                       | Modello TCP/IP               |
|----------------------------------|------------------------------|
| 7. Applicazione                  | 4. Applicazione              |
| 6. Presentazione                 |                              |
| 5. Sessione                      |                              |
| 4. Trasporto                     | 3. Trasporto                 |
| 3. Rete                          | 2. Internet                  |
| 2. Collegamento Dati            | 1. Link                      |
| 1. Fisico                        |                              |

🔍 TCP/IP accorpa i livelli 5-7 dell’OSI in uno solo → **Applicazione**  
🔍 I livelli fisico e data-link sono unificati in **Link**

---

## 🧰 Funzioni principali dei protocolli TCP/IP

| Funzione                      | Protocollo | Descrizione                                                                 |
|-------------------------------|------------|-----------------------------------------------------------------------------|
| **Indirizzamento logico**     | IP         | Ogni dispositivo ha un IP univoco. Usa subnetting e CIDR per organizzare la rete. |
| **Routing**                   | IP         | Ogni pacchetto trova il percorso corretto verso la destinazione, nodo per nodo. |
| **Controllo e gestione errori**| TCP        | Garantisce che i dati arrivino interi e in ordine. Gestisce anche il flusso. |
| **Supporto alle applicazioni**| TCP/UDP    | Le "porte" identificano servizi specifici (es. porta 80 per HTTP).         |
| **Risoluzione dei nomi**      | DNS        | Converte i nomi (es. `google.com`) in indirizzi IP.                        |

---

## 🎯 Conclusioni

✅ Il modello **OSI** ti aiuta a capire con precisione **dove avviene un problema** nella comunicazione.  
✅ Il modello **TCP/IP** è quello **realmente usato su Internet** ed è più semplice da memorizzare.

🎓 Studia entrambi. Analizzali. Ripassali.  
Sono la **base di ogni attacco e difesa in cybersecurity.**

