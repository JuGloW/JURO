# JuGloW Apps
> Aplikasi dalam Ekosistem JuGloW

## Overview
> Ringkasan

This directory contains all distributable applications within the JuGloW ecosystem.  
Each application represents a modular, reusable, and evolvable product built on top of JuGloW.

> Direktori ini berisi seluruh aplikasi yang dapat didistribusikan dalam ekosistem JuGloW.  
> Setiap aplikasi merupakan produk modular yang dapat digunakan ulang dan dikembangkan secara berkelanjutan di atas JuGloW.

Applications in this directory may include:
- End-user applications  
- Developer tools  
- Hybrid tools (GUI, CLI, and API-based)

> Aplikasi dalam direktori ini dapat berupa:
> - Aplikasi pengguna akhir  
> - Alat bantu pengembang  
> - Alat hibrida (GUI, CLI, dan API)

---

## Application and Source Separation
> Pemisahan Aplikasi dan Source Code

Applications distributed under `apps/` are intentionally separated from their raw source implementations, which reside in the `source/` directory.

> Aplikasi yang didistribusikan di `apps/` dipisahkan secara sengaja dari implementasi kode mentahnya yang berada di direktori `source/`.

This separation enables:
- Clean and stable distribution artifacts  
- Independent source evolution  
- Multiple build or packaging targets derived from the same source  

> Pemisahan ini memungkinkan:
> - Artefak distribusi yang bersih dan stabil  
> - Evolusi source secara independen  
> - Berbagai target build atau paket dari source yang sama

---

## Available Applications
> Aplikasi yang Tersedia

### 🎨 Design
**Application Directory:** [`apps/design/`](./design)

Visual and interface design tools within the JuGloW ecosystem.

> Alat desain visual dan antarmuka dalam ekosistem JuGloW.

**Related Source:** [`source/design/`](../source/design)

---

### 💻 Coding Editor
**Application Directory:** [`apps/coding-editor/`](./coding-editor)

Code editing tools optimized for structured, modular, and intent-based development.

> Alat editor kode yang dioptimalkan untuk pengembangan terstruktur, modular, dan berbasis intent.

**Related Source:** [`source/coding-editor/`](../source/coding-editor)

---

### 💬 ChatGlow
**Application Directory:** [`apps/chatglow/`](./chatglow)

AI-powered conversational interface integrated into JuGloW workflows.

> Antarmuka percakapan berbasis AI yang terintegrasi dalam alur kerja JuGloW.

**Related Source:** [`source/chatglow/`](../source/chatglow)

---

### 🖥️ Junhai Shell
**Application Directory:** [`apps/junhai-shell/`](./junhai-shell)

Shell and command-line environment designed for JuGloW-based systems.

> Lingkungan shell dan command-line yang dirancang untuk sistem berbasis JuGloW.

**Related Source:** [`source/junhai-shell/`](../source/junhai-shell)

---

### 🧠 Haicode
**Application Directory:** [`apps/haicode/`](./haicode)

Intent-oriented executable language tools and runtime environment.

> Alat bahasa eksekusi berbasis intent beserta runtime environment Haicode.

**Related Source:** [`source/haicode/`](../source/haicode)

---

## Application Directory Characteristics
> Karakteristik Direktori Aplikasi

Each application directory under `apps/` typically represents a distributable unit and may contain build outputs, assets, configuration, and metadata required for delivery.

> Setiap direktori aplikasi di bawah `apps/` merepresentasikan satu unit distribusi dan dapat berisi hasil build, aset, konfigurasi, serta metadata yang dibutuhkan untuk distribusi.

The internal structure of each application may vary depending on its purpose, platform, and delivery model.

> Struktur internal setiap aplikasi dapat berbeda tergantung tujuan, platform, dan model distribusinya.

---

## Ecosystem Philosophy
> Filosofi Ekosistem

JuGloW applications are designed with an emphasis on:

- Modular architecture  
- Clear separation between source and distribution  
- Long-term ecosystem scalability  
- Interoperability between human users and AI systems  

> Aplikasi JuGloW dirancang dengan penekanan pada:
> - Arsitektur modular  
> - Pemisahan yang jelas antara source dan distribusi  
> - Skalabilitas ekosistem jangka panjang  
> - Interoperabilitas antara manusia dan sistem AI


