**RecordStores.it** è una piattaforma open source dedicata alla mappatura, valorizzazione e gestione dei negozi di dischi indipendenti in Italia.

Il progetto nasce come iniziativa **community-driven**, con l’obiettivo di creare un archivio affidabile, curato e sostenibile nel tempo, costruito insieme ad appassionati, proprietari e contributor.

🌍 Sito ufficiale: https://www.recordstores.it

---

## ✨ Funzionalità principali

- 📍 Mappa interattiva dei negozi di dischi
- 🏪 Schede store complete (descrizione, immagini, orari, contatti)
- 👤 Sistema utenti (contributor, proprietari, admin)
- 🔐 Rivendicazione negozi con verifica email di dominio
- 🔔 Sistema notifiche interno
- ⭐ Preferiti e interazioni utente
- 🛠 Area amministrativa
- 🖼 Gallery immagini con ordinamento
- 🔗 Social links (Facebook, Instagram, YouTube, TikTok)

---

## 🧱 Stack tecnologico

- **Backend**: PHP 8.x (PDO, sessioni native)
- **Database**: MySQL / MariaDB
- **Frontend**: Bootstrap 5, Vanilla JavaScript
- **Mappe**: Leaflet
- **Email**: SMTP / mail abstraction
- **Auth**: Session-based + OAuth (Google)

---

## 📁 Struttura del progetto

```text
/
├── api/                # API backend
├── admin/              # Dashboard amministrativa
├── assets/             # JS, CSS, immagini statiche
├── lib/                # Helper e logica condivisa
├── templates/          # Componenti UI
├── sql/                # Schema database
├── config/             # Configurazioni (solo esempi)
└── README.md

## ⚙️ Installazione locale

1. Clona il repository

```bash
git clone https://github.com/TUO-USERNAME/recordstores.it.git
```

2. Crea il database

* MySQL / MariaDB
* importa lo schema da `sql/schema.sql`

3. Configura i file di esempio

```bash
cp config/db.php.example config/db.php
cp config/mail.php.example config/mail.php
cp config/oauth.php.example config/oauth.php
```

4. Avvia il server (MAMP, Apache, Nginx, ecc.)

---

## 🔐 Sicurezza

Questo repository **NON include**:

* credenziali reali
* email SMTP
* token OAuth
* dati utente
* media caricati dagli utenti

Tutti i file sensibili sono forniti **solo come `.example`**.

---

## 🤝 Contribuire

Contributi, issue e pull request sono benvenuti.

Linee guida:

* mantieni lo stile del codice
* commenta le parti critiche
* descrivi chiaramente lo scopo della PR

---


---

## 📜 Licenza

Questo progetto è rilasciato sotto **licenza MIT**.
Vedi il file `LICENSE` per i dettagli.

---

## ❤️ Credits

Sviluppo e design: **Recycle Design**.
Community: appassionati di musica e contributor indipendenti

> RecordStores.it è un progetto indipendente, non affiliato a piattaforme commerciali.

````
