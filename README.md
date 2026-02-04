# RecordStores.it

![PHP](https://img.shields.io/badge/PHP-8.x-blue)
![MySQL](https://img.shields.io/badge/MySQL-MariaDB-orange)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Active-success)
![Community](https://img.shields.io/badge/Community-Driven-purple)

**RecordStores.it** is an open-source platform dedicated to mapping, promoting, and managing independent record stores in Italy.

The project was born as a **community-driven initiative**, with the goal of building a reliable, curated, and long-term sustainable archive, created together with music lovers, store owners, and contributors.

🌍 Official website: https://www.recordstores.it

---

## ✨ Main Features

- 📍 Interactive map of record stores  
- 🏪 Detailed store profiles (description, images, opening hours, contacts)  
- 👤 User system (contributors, store owners, admins)  
- 🔐 Store claim system with domain email verification  
- 🔔 Internal notification system  
- ⭐ Favorites and user interactions  
- 🛠 Administrative dashboard  
- 🖼 Image gallery with ordering  
- 🔗 Social links (Facebook, Instagram, YouTube, TikTok)

---

## 🧱 Tech Stack

- **Backend**: PHP 8.x (PDO, native sessions)  
- **Database**: MySQL / MariaDB  
- **Frontend**: Bootstrap 5, Vanilla JavaScript  
- **Maps**: Leaflet  
- **Email**: SMTP / mail abstraction  
- **Auth**: Session-based + OAuth (Google)

---

## 📁 Project Structure

```text
/
├── api/                # Backend APIs
├── admin/              # Admin dashboard
├── assets/             # JS, CSS, static assets
├── lib/                # Shared helpers and logic
├── templates/          # UI components
├── sql/                # Database schema
├── config/             # Configuration (examples only)
└── README.md
└── README.md
````

---

## ⚙️ Local Installation

1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/recordstores.it.git
```

2. Create the database

* MySQL / MariaDB
* Import the schema from `sql/schema.sql`

3. Configure example files

```bash
cp config/db.php.example config/db.php
cp config/mail.php.example config/mail.php
cp config/oauth.php.example config/oauth.php
```

4. Start the server (MAMP, Apache, Nginx, etc.)

---

## 🔐 Security

This repository **does NOT include**:

* real credentials
* SMTP email accounts
* OAuth tokens
* user data
* uploaded media

All sensitive files are provided **only as `.example` files**.

---

## 🤝 Contributing

Contributions, issues, and pull requests are welcome.

Guidelines:

* keep code style consistent
* comment critical sections
* clearly describe the purpose of the PR

---

## 📜 License

This project is released under the **MIT License**.
See the `LICENSE` file for details.

---

## ❤️ Credits

Development & design: **Recycle Design**
Community: music lovers and independent contributors

> RecordStores.it is an independent project and is not affiliated with commercial platforms.

```
