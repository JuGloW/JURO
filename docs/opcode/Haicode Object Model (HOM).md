# ***Haicode — Intent-Oriented Executable Language***

-> **Bahasa Pemrograman Berorientasi Intent untuk Eksekusi Nyata**

---

## ***Overview***

**Haicode is an Intent-Oriented Executable Language based on Controlled Natural Language (CNL).**  
-> **Haicode adalah bahasa pemrograman berbasis Controlled Natural Language (CNL) yang berorientasi intent.**

**It is designed to bridge human semantic meaning with real execution (opcode / ABI).**  
-> **Bahasa ini dirancang untuk menjembatani makna semantik manusia dengan eksekusi nyata (opcode / ABI).**

**Haicode supports Indonesian and English as first-class languages.**  
-> **Haicode mendukung Bahasa Indonesia dan Bahasa Inggris sebagai bahasa utama.**

---

## ***Core Focus***

**Intent → natural meaning or human intention**  
-> **Intent → makna alami atau maksud manusia**

**Goal → high-level execution objective**  
-> **Goal → tujuan eksekusi tingkat tinggi**

**Opcode → real execution (runtime / ABI / native)**  
-> **Opcode → eksekusi nyata (runtime / ABI / native)**

---

## ***Ecosystem Integration***

**Haicode is designed for direct integration with:**  
-> **Haicode dirancang untuk integrasi langsung dengan:**

- **AI & multimodal processing**  
  -> **Pemrosesan AI & multimodal**
- **C ABI / native runtime**  
  -> **C ABI / runtime native**
- **External libraries such as redef, acruns, and JuGloW ecosystem**  
  -> **Library eksternal seperti redef, acruns, dan ekosistem JuGloW**

---

## ***Document Purpose***

**This document explains the evolution of Haicode grammar from v0.1 to v0.4.**  
-> **Dokumen ini menjelaskan evolusi grammar Haicode dari versi v0.1 hingga v0.4.**

**Including:**  
-> **Mencakup:**

- **Syntax changes**  
  -> **Perubahan sintaks**
- **Feature extensions**  
  -> **Ekstensi fitur**
- **Haicode Object Model (HOM) integration**  
  -> **Integrasi Haicode Object Model (HOM)**

---

# ***Core Concepts Summary***

---

## ***1️⃣ Intent — Semantic Meaning***

**Format: lowercase-word**  
-> **Format: kata-huruf-kecil**

**Intent represents natural meaning or conceptual intention.**  
-> **Intent merepresentasikan makna alami atau maksud konseptual.**

**Intent is never executed directly.**  
-> **Intent tidak pernah dieksekusi secara langsung.**

**It forms the semantic foundation of the language.**  
-> **Intent menjadi fondasi semantik bahasa.**

**Examples:**  
-> **Contoh:**

- `definisikan`
- `jalankan`
- `buat`

---

## ***2️⃣ Goal — Execution Objective***

**Format: CapitalizedWord**  
-> **Format: KataDenganHurufAwalKapital**

**Goal represents a high-level execution objective.**  
-> **Goal merepresentasikan tujuan eksekusi tingkat tinggi.**

**It binds intent to execution structure.**  
-> **Goal mengikat intent ke struktur eksekusi.**

**Goals may combine with role and scope.**  
-> **Goal dapat dikombinasikan dengan role dan scope.**

**Examples:**  
-> **Contoh:**

- `Definisikan`
- `Jalankan`
- `Jika`

---

## ***3️⃣ Opcode — Real Execution***

**Format: UPPERCASE_WORD**  
-> **Format: HURUF_KAPITAL_SEMUA**

**Opcode is a real runtime instruction executed by interpreter or native ABI.**  
-> **Opcode adalah instruksi runtime nyata yang dieksekusi oleh interpreter atau ABI native.**

**Opcode directly manipulates data, memory, file, or system.**  
-> **Opcode berinteraksi langsung dengan data, memori, file, atau sistem.**

**Examples:**  
-> **Contoh:**

- `CETAK`
- `JUMLAH`
- `BUKA_FILE`

---

# ***OPCODE Philosophy (Important)***

**Opcode in Haicode is NOT a CPU instruction or language-specific bytecode.**  
-> **Opcode dalam Haicode BUKAN instruksi CPU atau bytecode bahasa tertentu.**

**Opcode is a Universal Semantic Instruction Set.**  
-> **Opcode adalah Universal Semantic Instruction Set.**

**All languages map to the same OPCODE set via adapters.**  
-> **Semua bahasa memetakan ke OPCODE yang sama melalui adapter.**

---

## ***Intent vs Opcode***

**Intent defines what is meant.**  
-> **Intent mendefinisikan apa yang dimaksud.**

**Opcode defines what is executed.**  
-> **Opcode mendefinisikan apa yang dieksekusi.**

**No execution may occur without an opcode.**  
-> **Tidak ada eksekusi tanpa opcode.**

---

# ***Grammar & Technical Standards***

**Haicode grammar uses EBNF notation.**  
-> **Grammar Haicode menggunakan notasi EBNF.**

**Designed for cross-language compatibility.**  
-> **Dirancang untuk kompatibilitas lintas bahasa.**

**Fully integrated with Haicode Object Model (HOM).**  
-> **Terintegrasi penuh dengan Haicode Object Model (HOM).**

---

## ***Haicode Object Model (HOM)***

**HOM acts as a universal binding layer.**  
-> **HOM berfungsi sebagai lapisan pengikat universal.**

**It connects:**  
-> **Menghubungkan:**

- Python / C / native  
  -> **Python / C / native**
- File I/O  
  -> **File I/O**
- Error handling  
  -> **Penanganan error**
- Multimodal data (tensor for AI)  
  -> **Data multimodal (tensor untuk AI)**

---

# ***Grammar Evolution***

---

## ***v0.1 — Foundational Semantic Grammar***

**Primary focus:**  
-> **Fokus utama:**

- Intent / Goal / Opcode separation  
  -> **Pemisahan Intent / Goal / Opcode**

**Program structure:**  
-> **Struktur program:**

PROGRAM → EXECUTION → STATEMENT → CLAUSE


**Core rules:**  
-> **Aturan utama:**

- Intent → lowercase  
  -> **Intent → huruf kecil**
- Goal → Capitalized  
  -> **Goal → Kapital**
- Opcode → UPPERCASE  
  -> **Opcode → Kapital semua**

**Limitations:**  
-> **Keterbatasan:**

- No functions  
  -> **Belum ada fungsi**
- No loops  
  -> **Belum ada loop**
- No complex expressions  
  -> **Belum ada ekspresi kompleks**

---

## ***v0.2 — Structured Program & Expressions***

**Major upgrades:**  
-> **Upgrade utama:**

- Functions & classes  
  -> **Fungsi & kelas**
- Loops  
  -> **Loop**
- Math & logic expressions  
  -> **Ekspresi matematika & logika**

---

## ***v0.3 — Runtime, File I/O & Libraries***

**Major upgrades:**  
-> **Upgrade utama:**

- Runtime opcode  
  -> **Opcode runtime**
- File I/O  
  -> **File I/O**
- Error handling  
  -> **Penanganan error**
- Standard library  
  -> **Library standar**

---

## ***v0.4 — Full HOM & ABI Integration (Latest)***

**Major upgrades:**  
-> **Upgrade utama:**

- Full HOM integration  
  -> **Integrasi penuh HOM**
- C ABI bridge  
  -> **Jembatan ABI ke C**
- Module system  
  -> **Sistem modul**
- Multimodal & tensor support  
  -> **Dukungan multimodal & tensor**
- Executable generation  
  -> **Pembuatan executable**

---

# ***Version Comparison***

| Version | Main Focus |
|------|-----------|
| v0.1 | Intent / Goal / Opcode foundation |
| v0.2 | Functions, loops, expressions |
| v0.3 | Runtime, file I/O, libraries |
| v0.4 | HOM, ABI, modules, multimodal |

---

## ***Important Notes***

**All previous syntax remains valid.**  
-> **Semua sintaks lama tetap valid.**

**v0.4 is a unified evolution, not a breaking change.**  
-> **v0.4 adalah evolusi terpadu, bukan breaking change.**

---

# ***v0.4 Total Coverage***

- **100+ EBNF rules**  
  -> **100+ aturan EBNF**
- **Semantic execution model**  
  -> **Model eksekusi semantik**
- **Entity / role / scope system**  
  -> **Sistem entity / role / scope**
- **Runtime & native bridge**  
  -> **Jembatan runtime & native**
- **AI & multimodal support**  
  -> **Dukungan AI & multimodal**
- **Modular & extensible architecture**  
  -> **Arsitektur modular & dapat diperluas**
