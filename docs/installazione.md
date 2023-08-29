# Installazione del Progetto cs-ordini

## Introduzione

La documentazione del progetto cs-ordini fornisce informazioni dettagliate su come installare cs-ordini un sistema per la gestione degli Ordini professionali ed Associazioni basato su tecnologie come Ubuntu server 22, PHP 8.2, Phalcon 5.3, Docker, Vue.js, e altro ancora.

## Repository

Il progetto cs-odini è composto da diversi repository GitHub:
- **cs-ordini-os**: Contiene gli script per il sistema operativo Ubuntu Server 22. Gli script sono opzionali. Si può predisporre i servers utilizzando piattaforma equivalenti e compatibili.
- **cs-ordini-docker**: Fornisce i file Docker necessari per eseguire cs-ordini. Non tutti i docker sono obbligatori, sono solo indicativi per chiarire i requisiti della piattaforma. Si può configurare il cuore della piattaforma [cs-ordini-api](https://github.com/customsoft/cs-ordini-api)  per interfacciarsi con 
- **cs-ordini-vue**: Include i sorgenti per l'interfaccia utente basata su Vue.js per accedere alle API di cs-ordini.
- **cs-ordini-api**: Contiene il cuore della piattaforma ossia le API PHP, basate su framework Phalcon, per la gestione dei dati di cs-ordini.
- **cs-ordini-doc**: Contiene la documentazione stessa del progetto cs-ordini.

## Requisiti di Sistema

Per installare e utilizzare cs-ordini, è necessario soddisfare i seguenti requisiti:

- Sistema operativo: Ubuntu Server 22 o equivalente.
- PHP: Versione 8.2 o successiva.
- Framework PHP: Phalcon 5.3 o versione successiva.
- Browser Web: Per utilizzare l'interfaccia Vue.js, è necessario un browser moderno.
- Docker: Per semplificare la distribuzione e l'esecuzione dell'applicazione.

## Installazione

Segue una panoramica dell'installazione di cs-ordini:

- Visionare il repository cs-ordini-os e seguire le istruzioni per la configurazione del sistema operativo.

- Clonare il repository cs-ordini-docker e seguire le istruzioni per configurare e avviare i container Docker necessari.

- Configurare Apache per connettersi ai docker precedentemente creati
  - dominio.it -> web root dominio principale
  - api.dominio.it -> docker cs-ordini-api
  - documentale.dominio.it -> docker cs-ordini-cloud
  - ecc.

- Modificare i file di configurazione del docker cs-ordine-api

- Creare una nuova distributione dal docker cs-ordini-vue da collocare nella web root del dominio principale o copiare quella disponibile nella cartella /dist/ del docker [cs-ordini-vue](https://github.com/customsoft/cs-ordini-vue)

## Configurazione

Le istruzioni seguenti spiegano come configurare cs-ordini per l'uso:

- Nel repository cs-ordini-api, configurare l'accesso al database Maria DB e alle altre dipendenze.

- Nel repository cs-ordini-vue, configurare le impostazioni dell'interfaccia Vue.js per comunicare con le API di cs-ordini.

## Utilizzo

Dopo aver completato l'installazione e la configurazione, puoi iniziare a utilizzare cs-ordini:

- Accedi all'interfaccia Vue.js accedendo all'URL del dominio principale.
- Utilizza le funzionalità fornite dall'interfaccia per gestire gli ordini professionali e i dati degli associati.

## Contributi

Siamo aperti ai contributi! Se desideri contribuire a cs-ordini, consulta il repository cs-ordini-doc per ulteriori informazioni su come partecipare.
## Licenza

Il progetto cs-ordini è rilasciato sotto la licenza AGPL v3.0. Consulta il testo completo della licenza nel repository cs-ordini-doc.