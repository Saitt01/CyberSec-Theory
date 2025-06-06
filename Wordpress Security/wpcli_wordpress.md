# 📘Guida a WP-CLI – Gestione e Sicurezza di WordPress via Terminale

## 📌Cos’è WP-CLI

WP-CLI è un'interfaccia a riga di comando per WordPress.  
Ti permette di gestire completamente un sito WordPress scrivendo comandi nel terminale, invece di usare il pannello web (wp-admin).

Con WP-CLI puoi:

- Aggiornare WordPress, plugin e temi  
- Gestire utenti e ruoli  
- Eseguire backup del database  
- Attivare/disattivare plugin e temi  
- Riparare o verificare l'integrità del sito  

## 🎯Perché è utile per la sicurezza

### 1. Aggiornamenti rapidi

Puoi aggiornare core, plugin e temi con un solo comando, senza accedere al pannello.  
Questo riduce i rischi legati a vulnerabilità note non ancora patchate.

### 2. Meno uso del pannello admin (wp-admin)

Il pannello admin è una delle principali porte d’ingresso per attacchi brute force o tentativi di login.  
Usare WP-CLI significa interagire col sito in modo più sicuro, evitando l'esposizione del pannello web.

### 3. Gestione d'emergenza anche se il sito è offline

Se il sito va in crash o è bloccato da un plugin compromesso:

- Non riesci più ad accedere al pannello admin  
- Ma puoi accedere via terminale (SSH) e disattivare il plugin o tema che causa problemi con un comando WP-CLI

### 4. Automatizzazione di attività critiche

Con WP-CLI puoi automatizzare task importanti come:

- Aggiornamenti automatici  
- Backup giornalieri  
- Scansioni di sicurezza  

## 🔧Comandi Utili per la Sicurezza

### 🔄Aggiornamenti rapidi

wp core update // Aggiorna il core di WordPress all’ultima versione stabile.

wp plugin update --all // Aggiorna tutti i plugin installati.

wp theme update --all // Aggiorna tutti i temi WordPress.

### 🔍Verifica integrità del core

wp core verify-checksums // Confronta i file core di WordPress con quelli ufficiali.

### 🔐Gestione utenti

wp user list // Mostra l’elenco degli utenti del sito.

wp user delete ID --reassign=1 // Cancella un utente e riassegna i suoi contenuti a un altro utente.

wp user update ID --user_pass=NuovaPassword1234 // Cambia la password di un utente.

### 🧩Gestione plugin e temi

wp plugin list // Elenca tutti i plugin installati.

wp plugin deactivate nome-plugin // Disattiva un plugin specifico.

wp plugin delete nome-plugin // Cancella completamente un plugin.

prima: wp theme list,
successivamente: wp theme delete nome-tema // Visualizza e cancella i temi inutilizzati.

### 💾Backup del database

wp db export backup.sql // Crea un backup del database in formato .sql.

### ⚙️Automatizzare con cronjob

Esempio:
0 2 * * * wp plugin update --all >> /var/log/wp_updates.log // Esegue l’aggiornamento di tutti i plugin ogni notte alle 2:00 e salva i log in `/var/log/wp_updates.log`.