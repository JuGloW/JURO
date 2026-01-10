# JuGloW Apps
> Aplikasi dalam Ekosistem JuGloW

## Overview
> Ringkasan

This directory contains all distributable applications within the JuGloW ecosystem.  
Each application is designed as a modular, reusable, and evolvable component.

> Direktori ini berisi seluruh aplikasi yang dapat didistribusikan dalam ekosistem JuGloW.  
> Setiap aplikasi dirancang secara modular, dapat digunakan ulang, dan dikembangkan lebih lanjut.

Applications in this directory may be:
- End-user applications
- Developer tools
- Hybrid tools (GUI + CLI + API)

---

## App–Source Relationship
> Relasi Aplikasi dan Source Code

Each application in `apps/` has a corresponding raw source implementation inside the `source/` directory.

> Setiap aplikasi di `apps/` memiliki implementasi kode mentah yang bersesuaian di direktori `source/`.

Relationship model:

apps/<app-name>/
├─ README.md # App-level documentation
├─ build/ # Build or distribution artifacts
├─ assets/ # UI or media assets
├─ config/ # Configuration files
└─ package.* # Packaging metadata 



This separation allows:
- Clean distribution packages
- Independent source evolution
- Multiple build targets from the same source

> Pemisahan ini memungkinkan:
> - Paket distribusi yang bersih
> - Evolusi source secara independen
> - Banyak target build dari source yang sama

---

## Available Applications
> Aplikasi yang Tersedia

### 🎨 Design
**Folder:** [`apps/design/`](./design)

Visual and interface design tools for the JuGloW ecosystem.

> Alat desain visual dan antarmuka untuk ekosistem JuGloW.

**Source:** [`source/design/`](../source/design)

---

### 💻 Coding Editor
**Folder:** [`apps/coding-editor/`](./coding-editor)

Code editing tools optimized for structured, intent-based, and modular development.

> Alat editor kode yang dioptimalkan untuk pengembangan terstruktur, berbasis intent, dan modular.

**Source:** [`source/coding-editor/`](../source/coding-editor)

---

### 💬 ChatGlow
**Folder:** [`apps/chatglow/`](./chatglow)

AI-powered conversational interface integrated into the JuGloW ecosystem.

> Antarmuka percakapan berbasis AI yang terintegrasi ke dalam ekosistem JuGloW.

**Source:** [`source/chatglow/`](../source/chatglow)

---

### 🖥️ Junhai Shell
**Folder:** [`apps/junhai-shell/`](./junhai-shell)

Command-line and shell environment designed for JuGloW workflows.

> Lingkungan shell dan command-line yang dirancang untuk alur kerja JuGloW.

**Source:** [`source/junhai-shell/`](../source/junhai-shell)

---

### 🧠 Haicode
**Folder:** [`apps/haicode/`](./haicode)

Intent-oriented executable language tools and runtime environment.

> Alat bahasa eksekusi berbasis intent dan runtime environment Haicode.

**Source:** [`source/haicode/`](../source/haicode)

---

## Application Structure (Recommended)
> Struktur Aplikasi (Disarankan)

Each application directory may contain:



> Setiap direktori aplikasi dapat berisi struktur modular seperti di atas.

---

## Extensibility
> Ekstensibilitas

New applications can be added by:
1. Creating a new folder under `apps/`
2. Adding its corresponding raw source under `source/`
3. Registering the application in this README

> Aplikasi baru dapat ditambahkan dengan:
> 1. Membuat folder baru di `apps/`
> 2. Menambahkan source mentahnya di `source/`
> 3. Mendaftarkan aplikasi tersebut di README ini

---

## Philosophy
> Filosofi

JuGloW applications are built with principles of:

- Modular architecture  
- Clear separation between distribution and source  
- Human–AI interoperability  
- Long-term ecosystem scalability  

> Aplikasi JuGloW dibangun dengan prinsip:
> - Arsitektur modular
> - Pemisahan jelas antara distribusi dan source
> - Interoperabilitas manusia dan AI
> - Skalabilitas ekosistem jangka panjang



