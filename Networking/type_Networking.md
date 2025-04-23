# 🌐 Tipi di Reti 

## 📚 Introduzione

Le reti possono essere classificate in base a criteri come l’**estensione geografica**, la **tecnologia utilizzata** e le **funzionalità specifiche**. In ambito professionale è utile distinguere tra:
- **Terminologia comune**, usata nella pratica quotidiana;
- **Terminologia accademica**, utile per esami o documentazione tecnica.

---

## 🔖 Terminologia Comune

| Tipo di Rete | Descrizione |
|--------------|-------------|
| **WAN** (Wide Area Network) | Rete estesa su larga scala – Es: Internet |
| **LAN** (Local Area Network) | Rete locale – Es: casa, ufficio |
| **WLAN** (Wireless LAN) | LAN senza fili – Accesso via Wi-Fi |
| **VPN** (Virtual Private Network) | Connette più reti in modo sicuro via tunnel |

---

## 🌍 WAN – Wide Area Network

- Una **WAN** collega più LAN, anche a livello globale.
- **Internet** è la WAN più nota, ma non l’unica.
- Le WAN usano spesso **indirizzi pubblici** (non RFC 1918).
- Protocolli come **BGP** sono tipici nelle WAN.
- Alcune aziende gestiscono **WAN interne** (es. Intranet o reti air-gapped).

---

## 🏠 LAN / WLAN

- Una **LAN** assegna indirizzi IP privati (RFC 1918: `10.0.0.0/8`, `172.16.0.0/12`, `192.168.0.0/16`).
- Una **WLAN** è una LAN con accesso wireless, generalmente via Wi-Fi.
- In rari casi, LAN pubbliche (es: università, hotel) assegnano IP pubblici.

---

## 🔐 VPN – Virtual Private Network

Una VPN consente di accedere a una rete remota come se si fosse connessi fisicamente ad essa. Esistono tre tipi principali:

### 🧩 Site-to-Site VPN
- Connessione tra due reti tramite dispositivi di rete (router/firewall).
- Comune in ambienti aziendali multi-sede.

### 💻 Remote Access VPN
- Il client crea un’interfaccia virtuale per accedere alla rete remota.
- Esempio: **Hack The Box usa OpenVPN**.
- Tipologie:
  - **Split Tunnel**: solo traffico destinato alla rete remota passa dalla VPN.
  - **Full Tunnel**: tutto il traffico passa dalla VPN (più sicuro in ambito aziendale).

### 🌐 SSL VPN
- Accesso alla rete tramite **browser web**.
- Esempio: **Pwnbox** di HTB consente desktop remoto direttamente da browser.

---

## 📖 Terminologia Accademica

| Tipo di Rete | Descrizione |
|--------------|-------------|
| **GAN** (Global Area Network) | Rete globale – Es: Internet, reti aziendali mondiali |
| **MAN** (Metropolitan Area Network) | Rete metropolitana – Connette LAN su scala cittadina |
| **WPAN** (Wireless PAN) | Rete personale wireless – Es: Bluetooth |

---

## 🌐 GAN – Global Area Network

- Reti che collegano più WAN tra loro tramite **cavi sottomarini o satelliti**.
- Internet è la GAN più nota, ma anche alcune aziende gestiscono GAN private.
- L’infrastruttura è basata su **fibra ottica e backbone internazionali**.

---

## 🏙️ MAN – Metropolitan Area Network

- Connette LAN vicine in un’area geografica urbana.
- Utilizzata da aziende con più sedi in città.
- Linee dedicate e router ad alta capacità permettono **latenze simili a quelle di una LAN**.
- Può confluire in una WAN o GAN.

---

## 📱 PAN / WPAN – Personal Area Network

- **PAN**: rete personale connessa via cavo (es. USB).
- **WPAN**: rete personale wireless (es. Bluetooth, Wireless USB).
- Portata: pochi metri.
- Es: una **Piconet** Bluetooth collega dispositivi come cuffie, smartwatch, ecc.
- Utilizzate anche in contesti **IoT e domotica** (es: ZigBee, Z-Wave, Insteon).

---

📚 **Fonte**: Hack The Box Academy – Network Types  
✍️ **Autore**: Andrea Saitta  
📌 **Utilizzo**: Documentazione personale
