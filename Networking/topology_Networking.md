# 🔗 Topologie di Rete 

## 🧭 Definizione

La **topologia di rete** definisce la disposizione **fisica e logica** dei dispositivi interconnessi all’interno di una rete. I dispositivi (host), come client e server, comunicano attraverso componenti come **switch**, **router** e **bridge**, che gestiscono il traffico e garantiscono la connettività tra i nodi.

Le topologie possono essere:
- **Fisiche** → disposizione reale di cavi e dispositivi.
- **Logiche** → percorso dei dati, indipendente dalla struttura fisica.

---

## 📦 1. Tipi di Connessione

### 🔌 Connessioni cablate:
- Cavo coassiale
- Fibra ottica
- Cavo a coppie intrecciate (Twisted Pair)

### 📡 Connessioni wireless:
- Wi-Fi
- Reti cellulari (4G/5G)
- Satellitare

---

## 🔌 2. Nodi (Network Nodes)

Un **nodo** è un punto di accesso alla rete in grado di trasmettere o ricevere dati. Può essere un dispositivo intelligente (es. PC, router) o un componente passivo.

**Esempi di nodi:**
- Schede di rete (NIC)
- Ripetitori
- Hub
- Bridge
- Switch
- Router / Modem
- Gateway
- Firewall

---

## 🧩 3. Tipi di Topologie

La **struttura** delle connessioni tra i nodi può assumere diverse forme, fisiche o logiche. Le principali topologie sono:

---

### 🔸 Point-to-Point

- **Descrizione**: Collegamento diretto tra due dispositivi.
- **Esempio**: Linee dedicate, telefonia tradizionale.
- **Nota**: Non confondere con il modello Peer-to-Peer (P2P).

---

### 🔸 Bus

- **Descrizione**: Tutti i dispositivi condividono lo stesso mezzo trasmissivo.
- **Funzionamento**: Un host trasmette, gli altri ricevono e filtrano i pacchetti.
- **Svantaggio**: Il guasto al cavo centrale compromette tutta la rete.

---

### 🔸 Star (Stella)

- **Descrizione**: Tutti i nodi sono collegati a un componente centrale (hub, switch, router).
- **Vantaggio**: Facilmente scalabile e semplice da gestire.
- **Svantaggio**: Il nodo centrale è un punto di vulnerabilità critico.

---

### 🔸 Ring (Anello)

- **Descrizione**: Ogni nodo è collegato a due altri nodi, formando un anello.
- **Funzionamento**: I dati viaggiano in una sola direzione, spesso tramite un **token**.
- **Nota**: Può essere fisicamente un anello o logicamente simulato tramite una stella.

---

### 🔸 Mesh

- **Descrizione**: Ogni nodo è connesso a più altri nodi.
- **Tipologie**:
  - **Full Mesh**: ogni nodo è connesso a tutti.
  - **Partial Mesh**: solo alcuni nodi hanno connessioni multiple.
- **Vantaggi**: Alta disponibilità e ridondanza – ideale per WAN e MAN.

---

### 🔸 Tree (Albero)

- **Descrizione**: Gerarchia di topologie a stella.
- **Utilizzo**: Infrastrutture aziendali, MAN, grandi edifici.
- **Struttura**: Cablaggio strutturato e distribuzione multilivello.

---

### 🔸 Hybrid (Ibrida)

- **Descrizione**: Combinazione di due o più topologie di base.
- **Esempio**: Stella collegata tramite un backbone a bus.
- **Nota**: Due topologie identiche unite non costituiscono una topologia ibrida.

---

### 🔸 Daisy Chain (A Catena)

- **Descrizione**: I dispositivi sono collegati uno dopo l’altro in serie.
- **Utilizzo**: Automazione industriale (es. reti CAN).
- **Funzionamento**: Il segnale passa da nodo a nodo fino alla destinazione finale.

---

📚 **Fonte**: Hack The Box Academy – Introduction to Networking  
✍️ **Autore**: Andrea Saitta  
📌 **Utilizzo**: Documentazione e revisione personale 
