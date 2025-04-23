# 🔒 Proxies

## 🧠 Cos’è un proxy?

Un **proxy** è un dispositivo o servizio che si interpone tra un client e un server, fungendo da **mediatore** della comunicazione e spesso **analizzando o filtrando il traffico**.

🔑 La differenza rispetto a un gateway è che un proxy può **interagire con il contenuto dei pacchetti** (Layer 7 OSI), mentre un gateway si limita a smistarli.

---

## 💬 Percezione nei vari contesti

Il termine "proxy" viene interpretato in modo diverso a seconda del contesto:

- 🛡️ **Professionisti della sicurezza** → strumenti come **Burp Suite**, **SOCKS/SSH Proxy** (Chisel, sshuttle).
- 🌐 **Sviluppatori web** → servizi come **Cloudflare** o **ModSecurity** per filtrare il traffico.
- 👤 **Utenti comuni** → tool per cambiare posizione geografica (es. vedere Netflix USA).
- 🚔 **Forze dell’ordine** → spesso associato ad attività illecite o anonimato sospetto.

> ⚠️ **VPN ≠ Proxy**: spesso confuse, ma non equivalenti. Le VPN operano a livello di rete (Layer 3), i proxy a livello applicativo (Layer 7).

---

## 📍 Livello OSI

I proxy operano principalmente al **Livello 7 (Applicazione)** del modello OSI, gestendo protocolli come HTTP/HTTPS, DNS, SMTP, ecc.

---

## 📦 Tipi di Proxy

### 🔁 Forward Proxy (Proxy direzionale)

- ✅ **Funzionamento**: il client invia richieste → il proxy le inoltra → il server risponde → il proxy restituisce i dati al client.
- ✅ **Utilizzi comuni**:
  - Controllo dell’accesso a Internet.
  - Filtri contenuti (aziende, scuole).
  - Protezione da malware (limitando comunicazioni dirette).
  - Analisi del traffico (es. con **Burp Suite**).

💡 Browser come **Chrome/Edge/IE** usano il proxy di sistema.  
**Firefox**, invece, usa **libcurl**, e può richiedere configurazione manuale (utile per evitare malware proxy-aware).

---

### 🔄 Reverse Proxy

- 🔄 Inverte la logica: gestisce **richieste in entrata** e le smista a server interni.
- ✅ **Utilizzi**:
  - Protezione da attacchi DDoS.
  - Nascondere la struttura della rete interna.
  - **C2 channel** nei pentest, per inoltrare connessioni tramite host compromessi.

🔧 Esempi:
- **Cloudflare** → protezione + caching.
- **ModSecurity** → Web Application Firewall.

---

### 🕵️‍♂️ Transparent vs Non-Transparent Proxy

| Tipo               | Descrizione                                                                 |
|--------------------|------------------------------------------------------------------------------|
| **Transparent**     | Il client **non è consapevole** del proxy; il traffico viene intercettato. |
| **Non-Transparent** | Il client **deve essere configurato** per instradare il traffico attraverso il proxy. |

---

📚 **Fonte**: Hack The Box Academy – Proxies  
✍️ **Autore**: Andrea Saitta 
📌 **Uso**: Documentazione personale 
