
# RecordStores.it

![PHP](https://img.shields.io/badge/PHP-8.x-blue)
![MySQL](https://img.shields.io/badge/MySQL-MariaDB-orange)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Active-success)
![Community](https://img.shields.io/badge/Community-Driven-purple)

**RecordStores.it** is an open-source platform dedicated to mapping, promoting, and managing independent record stores in Italy.

The project was born as a **community-driven initiative**, with the goal of building a reliable, curated, and long-term sustainable archive, created together with music lovers, store owners, and contributors.

🌍 Official website: [https://www.recordstores.it](https://www.recordstores.it)

---

## ✨ Main Features

* 📍 Interactive map of record stores
* 🏪 Detailed store profiles (description, images, opening hours, contacts)
* 👤 User system (contributors, store owners, admins)
* 🔐 Store claim system with domain email verification
* 🔔 Internal notification system
* ⭐ Favorites and user interactions
* 🛠 Administrative dashboard
* 🖼 Image gallery with ordering
* 🔗 Social links (Facebook, Instagram, YouTube, TikTok)

### 🎟 Events System (New)

* 📅 Community-driven event proposals
* 🏬 Events linked to stores or custom venues
* 🖼 Optional event image upload (with default placeholder fallback)
* ⏳ Admin moderation workflow (pending / approved / rejected)
* 🔔 Automatic notifications:

  * to admins when a new event is submitted
  * to users when their event is approved or rejected
* 🧭 Smart filtering:

  * Today
  * Weekend
  * This Month
  * All Events
* 🏙 Dynamic city filter (auto-generated from available events)
* 🖱 Swiper-based responsive carousel for multi-event months
* 📖 Expandable descriptions with smooth animation
* 🔗 External event link support

---

## 🧱 Tech Stack

* **Backend**: PHP 8.x (PDO, native sessions)
* **Database**: MySQL / MariaDB
* **Frontend**: Bootstrap 5, Vanilla JavaScript
* **Maps**: Leaflet
* **Carousel**: Swiper.js
* **Email**: SMTP / mail abstraction
* **Auth**: Session-based + OAuth (Google)

---

## 📁 Project Structure

```text
/
├── api/                # Backend APIs (stores, events, notifications)
│   ├── admin/          # Admin-only APIs
│   └── events/         # Event management APIs
├── admin/              # Admin dashboard & moderation panels
├── assets/             # JS, CSS, static assets
├── uploads/            # Uploaded images (stores, events)
├── lib/                # Shared helpers and business logic
├── templates/          # UI components
├── sql/                # Database schema
├── config/             # Configuration (examples only)
└── README.md
```

---

## 🎟 Events Workflow

### 1️⃣ Submission

Authenticated users can propose a new event via modal form.

The event is saved with:

```
status = 'pending'
```

### 2️⃣ Admin Moderation

Admins can:

* Approve → `status = 'approved'`
* Reject → `status = 'rejected'`

Moderation panel:

```
/admin/events-pending.php
```

### 3️⃣ Notifications

When an event is:

* **Submitted**

  * Admins receive notification
  * User receives confirmation notification

* **Approved**

  * User receives approval notification

* **Rejected**

  * User receives rejection notification

Notifications are stored internally and displayed via the notification system.

---

## 🖼 Image Handling (Events)

* Event image upload is optional.
* If no image is provided:

  * A predefined placeholder image is automatically used.
* Images are stored inside:

```
/uploads/events/
```

Frontend rendering dynamically resolves:

```
BASE_URL/uploads/events/{image}
```

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

4. Ensure uploads directory exists

```bash
mkdir uploads
mkdir uploads/stores
mkdir uploads/events
```

5. Start the server (MAMP, Apache, Nginx, etc.)

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

---
