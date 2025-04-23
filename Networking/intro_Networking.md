# 🌐 Panoramica sul Networking 

## 📘 Cos’è una rete?

Una rete consente a due o più computer di comunicare tra loro per condividere dati, risorse e servizi. Esistono diverse **topologie** (mesh, albero, stella), **mezzi di trasmissione** (Ethernet, fibra ottica, coassiale, wireless) e **protocolli** (TCP, UDP, IPX) che rendono possibile la comunicazione.

Per un professionista della sicurezza informatica, la comprensione del networking è cruciale: **un errore silente di rete può compromettere l’intera analisi** o lasciare spazio ad attacchi non rilevati.

---

## 🛡️ Reti Flat vs Reti Segmentate

Una rete piatta (*flat network*) è semplice da configurare, ma poco sicura: tutti i dispositivi sono sullo stesso livello, senza separazione logica.

Segmentare la rete in **sottoreti dedicate** consente di:
- applicare regole granulari,
- migliorare il monitoraggio,
- rallentare l’attaccante in caso di compromissione.

### 🔲 Esempio 1 – ACL e Segmentazione
Implementare ACL tra le sottoreti equivale a **circondare una proprietà con recinzioni e punti di accesso controllati**.  
> Es: Perché la rete delle stampanti comunica con i server via HTTP?

### 💡 Esempio 2 – Documentazione della rete
Documentare lo scopo di ogni rete è come **installare luci di sicurezza attorno a una proprietà**.  
> Es: Perché la stampante comunica con Internet?

### 🌿 Esempio 3 – IDS
Strumenti come **Snort** o **Suricata** sono come **siepi sotto le finestre**: ostacolano e rendono più visibile lo scanning di rete.

---

## 🧠 Errore comune nei Pentest – La subnet /24

Molti penetration tester assumono erroneamente che la rete utilizzi una subnet `/24` (255.255.255.0). Questo può portare a **false interpretazioni**, ad esempio credere che un server sia offline quando in realtà è solo su un'altra subnet.

### 🔍 Caso pratico:
| Dispositivo          | Indirizzo IP           |
|----------------------|------------------------|
| Gateway Server       | `10.20.0.1/25`         |
| Domain Controller    | `10.20.0.10/25`        |
| Gateway Client       | `10.20.0.129/25`       |
| Workstation          | `10.20.0.200/25`       |
| Pentester            | `10.20.0.252/24`       |

Il pentester riusciva a comunicare con i client, ma non con il Domain Controller (su subnet diversa), e ha **erroneamente concluso** che il DC fosse offline.

---

## 🏠 Comunicazione tra rete domestica e aziendale

Scenario: vuoi visitare un sito aziendale da casa.

1. Il tuo dispositivo invia la richiesta tramite il **router** → ISP.
2. L’**ISP** consulta il **DNS** per ottenere l’IP dell’indirizzo digitato.
3. Il pacchetto viene inoltrato al **server web aziendale**.
4. Il server risponde → risposta inoltrata al tuo IP → pagina caricata.

### 🔗 Differenza FQDN vs URL (esempio):
- **FQDN**: `www.hackthebox.eu` → indirizzo del “palazzo”.
- **URL**: `https://www.hackthebox.eu/example?floor=2&office=dev&employee=17` → specifica anche “piano”, “ufficio” e “persona”.

---

## 🔐 Segmentazione ideale di una rete aziendale

Una segmentazione efficace può prevenire numerose vulnerabilità:

1. **Web Server in DMZ**  
   Separato dalla rete interna: esposto a Internet → alto rischio di compromissione.

2. **Workstation su rete dedicata**  
   Nessuna comunicazione diretta tra workstation → previene attacchi MITM e lateral movement.

3. **Switch e Router in rete di amministrazione**  
   Riduce il rischio di sniffing e attacchi OSPF spoofing.

4. **IP Phone su VLAN separata**  
   Migliore gestione della latenza + sicurezza contro eavesdropping.

5. **Stampanti su rete isolata**  
   Difficili da proteggere → rischi di NTLM relay, persistence e leakage.

---

📚 **Fonte**: Hack The Box Academy – Networking Overview  
✍️ **Autore**: Andrea Saitta  
📌 **Utilizzo**: Documentazione personale 
