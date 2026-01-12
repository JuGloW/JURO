# Haicode Rules OPCODE Structure 
> # Aturan Haicode Struktur OPCODE
 
## Overview 
This directory (`opcode/rules/`) is a placeholder for rules-related components in Haicode's OPCODE system. It supports the intent-oriented execution model, where **uppercase words** represent **rules** (conditional logic), **lowercase words** represent **intent** (semantic triggers for meaning), and **capitalized words** represent **goal** (high-level objectives). This structure ensures semantic clarity and operational efficiency, aligning with Haicode's grammar rules from v0.1 to v0.4. 
> ## Ringkasan
Direktori ini (`opcode/rules/`) berfungsi sebagai tempat penyimpanan komponen yang berkaitan dengan aturan dalam sistem OPCODE Haicode. Struktur ini mendukung model eksekusi berorientasi niat, di mana **kata-kata huruf besar** mewakili **aturan** (logika kondisional), **kata-kata huruf kecil** mewakili **niat** (pemicu semantik untuk makna), dan **kata-kata huruf kapital** mewakili **tujuan** (tujuan tingkat tinggi). Struktur ini memastikan kejelasan semantik dan efisiensi operasional, sesuai dengan aturan tata bahasa Haicode dari v0.1 hingga v0.4.
 
## Rules Semantic Rules 
Based on Haicode's grammar: 
- **Uppercase Word**: Rules (conditional logic) - Represents rules for execution control. Examples: "JUMLAH" (addition rules), "Cetak" (print rules). 
- **Lowercase Word**: Intent (maksud) - Represents semantic triggers for natural language processing. Examples: "jumlah" (addition intent), "cetak" (print intent). 
- **Capitalized Word**: Goal (tujuan) - Represents high-level objectives. Examples: "Jumlah" (addition goal), "Cetak" (print goal). 
> ## Aturan Semantik
Berdasarkan tata bahasa Haicode:
- **Kata Huruf Besar**: Aturan (logika kondisional) - Mewakili aturan untuk pengendalian eksekusi. Contoh: "JUMLAH" (aturan penjumlahan), "Cetak" (aturan cetak).
- **Kata Huruf Kecil**: Maksud (intent) - Mewakili pemicu semantik untuk pemrosesan bahasa alami. Contoh: "jumlah" (maksud penjumlahan), "cetak" (maksud cetak).
- **Kata dengan Huruf Kapital**: Tujuan (tujuan) - Mewakili tujuan tingkat tinggi. Contoh: "Jumlah" (tujuan penjumlahan), "Cetak" (tujuan cetak).
 
This follows semantic rules from controlled natural language programming, where rules drive conditional intent, and intent triggers opcode.
[pypi.org](https://pypi.org/project/intentlang/0.2.7/)
> Ini mengikuti aturan semantik dari pemrograman bahasa alami yang terkontrol, di mana aturan menggerakkan niat kondisional, dan niat memicu opcode.
 
## Structure 
- **Purpose**: Store rules definitions, mappings, and documentation for rules-to-opcode resolution. 
- **Current Status**: Empty (struktur saja) - Intended for future expansion with rules files (e.g., rules_map.py, conditional_rules.py). 
- **Integration**: Links to Haicode grammar v0.1-v0.4 for rules parsing and execution dispatch. 
> ## Struktur
- **Tujuan**: Menyimpan definisi aturan, pemetaan, dan dokumentasi untuk resolusi aturan ke opcode.
- **Status Saat Ini**: Kosong (hanya struktur) - Ditujukan untuk perluasan di masa depan dengan berkas aturan (misalnya, rules_map.py, conditional_rules.py).
- **Integrasi**: Terhubung ke tata bahasa Haicode v0.1-v0.4 untuk parsing aturan dan pengiriman eksekusi.
 
## Usage 
To use: 
1. Add rules files to this directory (e.g., for new conditional triggers). 
2. Register rules in `opcode/registry.py` for semantic resolution. 
3. Test with Haicode programs: `Jika "data" None Jalankan "Cetak" "Hello World"!.` 
> ## Penggunaan
Untuk menggunakan:
1. Tambahkan berkas aturan ke direktori ini (misalnya, untuk pemicu kondisional baru).
2. Daftarkan aturan di `opcode/registry.py` untuk resolusi semantik.
3. Uji dengan program Haicode: `Jika "data" None Jalankan "Cetak" "Hello World"!.`
 
## Examples from Haicode Grammar 
From v0.1-v0.4: 
- Rules: "JUMLAH" (uppercase) → Intent: "jumlah" (lowercase) → Goal: "Jumlah" (capitalized) → Opcode: "JUMLAH". 
- Rules: "Cetak" (uppercase) → Intent: "cetak" (lowercase) → Goal: "Cetak" (capitalized) → Opcode: "Cetak". 
> ## Contoh dari Grammar Haicode
Dari v0.1-v0.4:
- Aturan: "JUMLAH" (huruf besar) → Niat: "jumlah" (huruf kecil) → Tujuan: "Jumlah" (huruf besar) → Opcode: "JUMLAH".
- Aturan: "Cetak" (huruf besar) → Niat: "cetak" (huruf kecil) → Tujuan: "Cetak" (huruf besar) → Opcode: "Cetak".
 
This structure enables universal instruction sets across languages, from rules to opcode.
[stackoverflow.com](https://stackoverflow.com/questions/18762446/x86-jmp-opcode-structure)
> Struktur ini memungkinkan set instruksi universal di seluruh bahasa, dari aturan hingga opcode.
 
## Contributing 
- Add rules files for new triggers. 
- Update rules for v0.5+ grammar. 
- Test with Haicode executor. 
> ## Kontribusi
- Tambahkan berkas aturan untuk pemicu baru.
- Perbarui aturan untuk tata bahasa v0.5+.
- Uji dengan eksekutor Haicode.
 
For more details, see Haicode documentation. 
> Untuk detail lebih lanjut, lihat dokumentasi Haicode
