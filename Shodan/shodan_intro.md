# 🔍 Shodan – Introduzione

## 🧠 Cos'è Shodan?

Shodan è come un google, quindi un motore di ricerca, ma anzichè indicizzare pagine web esso **fornisce informazioni sui dispositivi connessi online** come:

- Server
- Router
- Webcam
- Sistemi di controllo industriale 
- Altri dispositivi IoT

È uno strumento **potentissimo** per la sicurezza informatica perché consente di trovare:

- Sistemi non aggiornati
- Sistemi con credenziali predefinite
- Servizi aperti
- Vulnerabilità note
- Mapping di network
- E molto altro..

Grazie a **filtri avanzati**, è possibile effettuare ricerche mirate su:

- Sistema operativo
- Versioni software
- Produttori specifici
- Servizi esposti
- Altro ancora..

> 🔎 Oltre alla cybersecurity, viene utilizzato anche in **ricerche di mercato**, ad esempio per analizzare la distribuzione geografica dei dispositivi connessi.

## 🛡️ A cosa serve Shodan in Cybersecurity?

Shodan è uno strumento fondamentale per i **pentester** e gli **analisti di sicurezza**, utilizzato nella fase di **Information Gathering** e nello scoprire vulnerabilità prima che esse vengano sfruttate da malintenzionati!

Tuttavia, come ogni strumento potente, può essere usato anche con scopi **malevoli** in modo diretto ed indiretto, ad esempio:

- Ampliamento botnet per attacchi DDoS
- Cyberterrorismo
- Furti di dati
- Social engineering

---

## 🚀 Come iniziare con Shodan

1. Registrati su: [https://www.shodan.io/](https://www.shodan.io/)
2. Una volta registrato, otterrai una **API Key gratuita**
3. Il piano gratuito ha funzionalità molto limitate, in particolare queste funzionalità includono:

     - Ricerca per parole chiave senza filtri avanzati (L'utilizzo di filtri specifici come per esempio 'port:'/'hostname'/'os': costa dei crediti che non si hanno con memb. gratuita)
     - Visualizzare risultati ma in numero limitato
     - Esplorazione di ricerche popolari, es. 'webcam' ma si potrà ottenere solamente qualche risultato campione

### ❌ Limiti del piano gratuito:

-  Niente filtri avanzati (`port:`, `os:`, `hostname:`, `vuln:`, ecc.)
-  Risultati limitati per ogni ricerca
-  Niente **scansione on-demand** su IP/network
-  Niente **monitoraggio** IP/host (alert)
-  Niente **download/esportazione** dei dati
-  Accesso molto limitato a mappe e trend


## 🧪 Shodan API (Free)

Ogni utente registrato, dispone di una API Key gratuita associata al proprio account, la quale consente di utilizzare l'API Shodan & i tool CLI.
Per i limiti l'API rispetta lo stesso sistema di crediti dell'interfaccia web, 0 crediti = 0 chiamate API che richiedono crediti.

> 📌 Documentazione ufficiale: [https://developer.shodan.io/api](https://developer.shodan.io/api)

Con la versione gratuita puoi:

- Recuperare info da un IP:
curl -X GET "https://api.shodan.io/shodan/host/{IP_TARGET}?key=API_KEY"

- Contare servizi o host:
shodan count port:x

#### Oltre alla classica REST API (che richiede la API key), Shodan mette a disposizione alcuni servizi API pubblici gratuiti che non richiedono nemmeno autenticazione e sono pensati per fornire informazioni di base rapidamente (separate dalle funzionalità complete del motore di ricerca principale): 

🌐 InternetDB:
è un servizio che restituisce in forma ridotta le informazioni sulle porte aperte e vulnerabilità note di un IP specifico, es. di utilizzo:

curl https://internetdb.shodan.io/{ip} - (Documentazione Ufficiale: https://internetdb.shodan.io/)

🛰️ Geonet:
Utile ad effettuare ping e DNS lookup da varie location globali  - (Documentazione Ufficiale: https://geonet.shodan.io/docs#/)

🔓 Shodan CVE Database:
Ossia un database pubblico di vulnerabilità CVE consultabile via web (cvedb.shodan.io) e API (Guarda: https://cvedb.shodan.io/ & https://cvedb.shodan.io/docs)

🧩 Shodan Add-ons (Browser Extensions):
Plugin che una volta installati mostrano automaticamente le informazioni sulle porte aperte per il sito web che si sta visitando, sfruttando l’API InternetDB in background.

### 🧪 Esempi pratici di query gratuite:
**apache**
Cerca tutti i dispositivi con HTTP banner contenente “Apache”

**"Default password"**
Cerca la frase nei banner, utile per trovare interfacce con credenziali di default

**webcamXP**
Trova feed video live da webcam che usano questo software

**"DVR Login"**
Individua sistemi di videosorveglianza esposti online

**SSH-2.0-OpenSSH**
Mostra host con porta 22 aperta che usano OpenSSH

**shodan count port:x**
Conta quanti host nel database Shodan hanno la porta x aperta

🧩 Conclusioni
🔓 La versione gratuita di Shodan è perfetta per iniziare a esplorare, sperimentare e comprendere il funzionamento dello strumento.
Per ottenere il massimo, soprattutto per progetti professionali, è necessario un upgrade del piano.
