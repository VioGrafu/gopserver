# 🚀 GopServer — Universal Multi-Database REST API Server

![Go Version](https://img.shields.io/badge/Language-Go-00ADD8?style=for-the-badge&logo=go)
![License](https://img.shields.io/badge/License-Commercial_OEM_Lifetime-orange?style=for-the-badge)
![Version](https://img.shields.io/badge/Version-1.0.0-green?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Windows_|_Linux_|_macOS-blue?style=for-the-badge)

**GopServer** is a high-performance REST API engine written in **Go** that allows you to expose any relational database as a full-featured API without writing a single line of backend code. Just configure it once and get instant access to CRUD operations, advanced filtering, and robust security.



## 🎯 Who is it for?

GopServer was built to eliminate repetitive backend tasks and is ideal for:

* **Full-Stack & Frontend Developers**: For those who want to focus on the UI/UX and need a production-ready, stable, and secure backend immediately.
* **Database Administrators (DBAs)**: For professionals who need to expose specific database tables via API (PostgreSQL, MySQL, MSSQL, Oracle) without developing new applications from scratch.
* **Prototypes & MVPs**: Perfect for rapidly launching a project where speed of implementation is critical.
* **Legacy System Integration**: Companies looking to connect older databases (like Oracle or MSSQL) to modern web or mobile apps.
* **Automation & Scripting**: For users needing a centralized, secure point of access to data using static tokens or JWT.

## ✨ Key Features

* **Zero Code & No Recompile**: Adding a new table is as simple as editing a JSON file; no server recompilation required.
* **Multi-Database Support**: Out-of-the-box support for PostgreSQL (12+), MySQL/MariaDB (5.7+), SQLite (3.x), MSSQL (2012+), and Oracle (12c R2+).
* **Robust Authentication**: Integrated support for JWT (Bearer tokens), session-based cookies for web apps, and static tokens for server-to-server integrations.
* **Advanced Filtering & Sorting**: Powerful URL-based filtering using operators like `exact`, `contains`, `gt`, `lt`, `isnull`, and more.
* **Granular Security**: Hide (`hidden`) or lock (`locked`) sensitive fields like passwords or timestamps directly via configuration.
* **Environment Variables**: Support for `${VAR_NAME}` syntax in configuration to keep credentials secure.
* **Rate Limiting**: Built-in brute-force protection for authentication endpoints.
* **Lightweight & Portable**: A single ~11MB static binary with no external dependencies required.



## 📊 Supported Databases

| Engine | Min. Version | Default Port | Notes |
| :--- | :--- | :--- | :--- |
| **PostgreSQL** | 12+ | 5432 | Fully supported |
| **MySQL / MariaDB** | 5.7+ / 10.3+ | 3306 | Fully supported |
| **SQLite** | 3.x | — | File-based, no server needed |
| **MS SQL Server** | 2012+ | 1433 | Fully supported |
| **Oracle** | 12c R2+ | 1521 | Service name required |

## 🛠️ Quick Start

1.  **Download** the binary for your OS from [Releases](https://github.com/viorel-grafu/gopserver/releases).
2.  **Configure** your database connection in `conf/app.conf`.
3.  **Define** the tables to be exposed in `conf/tables.json`.
4.  **Run** the server:
    * **Windows**: `gopserver.exe`
    * **Linux/macOS**: `./gopserver`
5.  **Verify**: Access `http://localhost:8080/health`.

## 🔑 Licensing (Commercial OEM Lifetime)

GopServer operates in two modes:

* **Demo Mode**: Active without a license key. Limits GET results to 3 records and disables POST, PUT, and DELETE operations.
* **Full Mode (Commercial OEM Lifetime)**: Requires a valid license key tied to your hardware (HWID). Once activated, the license is permanent (lifetime) for that specific machine/hardware.

To activate, run `POST /activate` to get your **HWID** and contact the vendor.

## 📖 Full Documentation

For the detailed configuration guide, API reference, and `curl` examples, visit our official site:
👉 **[https://api-server.app](https://api-server.app)**

---
© 2026 GopServer. All rights reserved.
