Haicode — Intent-Oriented Executable Language

Haicode adalah bahasa pemrograman berbasis Controlled Natural Language (CNL) yang intent-oriented, dirancang untuk menjembatani makna semantik manusia dengan eksekusi 
nyata (opcode / ABI).

Bahasa ini mendukung Bahasa Indonesia dan Inggris, serta berfokus pada:

Intent → makna atau maksud alami

Goal → tujuan eksekusi tingkat tinggi

Opcode → eksekusi nyata (runtime / ABI / native)

Haicode dikembangkan untuk integrasi langsung dengan:

AI & multimodal processing

C ABI / native runtime

Library eksternal seperti redef, acruns, dan ekosistem JuGloW

Dokumen ini menjelaskan evolusi grammar Haicode dari v0.1 hingga v0.4, termasuk:

Perubahan sintaksis

Ekstensi fitur

Integrasi Haicode Object Model (HOM)

Ringkasan Konsep Inti
1. Intent — Makna Semantik

Format: lowercase-word

Intent merepresentasikan maksud alami atau konsep dasar, seperti kata kerja atau ide utama.

Tidak dieksekusi langsung

Menjadi fondasi semantik bahasa

Contoh:

definisikan
jalankan
buat

2. Goal — Tujuan Eksekusi

Format: CapitalizedWord

Goal merepresentasikan aksi atau tujuan tingkat tinggi yang mengarahkan alur eksekusi.

Mengikat intent ke struktur eksekusi

Dapat dikombinasikan dengan role & scope

Contoh:

Definisikan
Jalankan
Jika

3. Opcode — Eksekusi Nyata

Format: UPPERCASE_WORD

Opcode adalah instruksi runtime nyata yang dieksekusi oleh interpreter atau native runtime (ABI).

Langsung dieksekusi

Berinteraksi dengan data, memori, file, atau C ABI

Contoh:

CETAK
JUMLAH
BUKA_FILE

Grammar & Standar Teknis

Menggunakan EBNF Notation

Dirancang untuk kompatibilitas lintas bahasa

Terintegrasi penuh dengan Haicode Object Model (HOM)

HOM berfungsi sebagai pengikat universal untuk:

Python / C / native

File I/O

Error handling

Multimodal data (tensor untuk AI)

Semua versi v0.1–v0.4 kompatibel, dengan v0.4 sebagai versi terbaru.

Evolusi Grammar Haicode
v0.1 — Foundational Semantic Grammar

Fokus utama:
Dasar semantik Intent / Goal / Opcode

Struktur Program:

PROGRAM → EXECUTION → STATEMENT → CLAUSE


Aturan Utama:

Intent → lowercase

Goal → Capitalized

Opcode → UPPERCASE

Fitur Kunci:

Entity system (known / unknown)

Role (core, system, user, ai)

Scope & path

Conditional dasar

Action (create, run, generate)

Contoh:

Definisikan "data" kedalam (path) [ai].
Jalankan "Cetak" "Hello World"!.


Keterbatasan:

Belum ada fungsi, loop, atau ekspresi kompleks

v0.2 — Structured Program & Expressions

Upgrade Utama:

Fungsi

Kelas

Loop

Ekspresi matematika & logika

Fitur Tambahan:

Operator: + - * / > < == !=

Function & class definition

Loop: Ulangi, Selama, Untuk setiap

Contoh:

FUNGSI tambah(a:angka, b:angka):angka {
  nilai hasil = a + b.
  KEMBALIKAN hasil.
}.
PANGGIL tambah(2, 3).

v0.3 — Runtime, File I/O & Libraries

Upgrade Utama:

Runtime opcode

File I/O

Error handling

Standard library

Integrasi redef & acruns

Fitur Kunci:

File I/O (BUKA_FILE, BACA_FILE, TULIS_FILE)

Error handling (Coba, Tangkap, Akhirnya)

Standard ops (JUMLAH, KALI, PENGGAL)

Library import

Contoh:

IMPORT redef.
BUKA_FILE "data.txt" sebagai file.
BACA_FILE file ke konten.
Cetak konten!.

v0.4 — Full HOM & ABI Integration (Latest)

Upgrade Utama:

Integrasi penuh Haicode Object Model (HOM)

ABI bridge ke C

Module system

Multimodal (tensor)

Executable generation

Fitur Baru:

hom . IDENTIFIER → akses HOM

abi . UPPERCASE_WORD → C ABI

Module import/export

Tensor processing untuk AI

Metadata executable

Contoh:

MODULE AI {
  IMPORT redef.
  export tensor_ai.
}.

hom . "ai" . "proses_tensor"(data) [ai].

Ringkasan Perbandingan Versi
Versi	Fokus Utama
v0.1	Dasar intent / goal / opcode
v0.2	Fungsi, loop, ekspresi
v0.3	Runtime, file I/O, library
v0.4	HOM, ABI, modul, multimodal

Catatan Penting:

Semua sintaks lama tetap valid

v0.4 adalah unified evolution, bukan breaking change

Cakupan Total v0.4

100+ aturan EBNF

Semantic execution model

Entity / role / scope system

Runtime & native bridge

AI & multimodal support

Modular & extensible architecture
