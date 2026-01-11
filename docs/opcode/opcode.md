# ***OPCODE Core Files — Detailed Architecture Documentation***
-> **File Inti OPCODE — Dokumentasi Arsitektur Mendalam**

---

## ***File 1: opcode/__init__.py***

### ***Description***

**This file initializes the `opcode` directory as a Python package.**  
-> **File ini menginisialisasi direktori `opcode` sebagai Python package.**

**It allows modules inside the directory to be imported properly.**  
-> **Hal ini memungkinkan modul di dalam direktori dapat diimpor dengan benar.**

**Examples include opcode.py, opcode_base.py, and related modules.**  
-> **Contohnya termasuk opcode.py, opcode_base.py, dan modul terkait lainnya.**

---

### ***Purpose***

**The file itself can be empty and serves as a package marker.**  
-> **File ini dapat kosong dan berfungsi sebagai penanda package.**

**It enables Python to recognize OPCODE as an organized module collection.**  
-> **Ini memungkinkan Python mengenali OPCODE sebagai kumpulan modul terorganisir.**

**Although optional, it is recommended for package-level initialization.**  
-> **Meskipun opsional, file ini direkomendasikan untuk inisialisasi tingkat package.**

---

### ***Key Roles***

- **Marks the directory as a Python package**  
  -> **Menandai direktori sebagai package Python**

- **Supports modular OPCODE architecture**  
  -> **Mendukung arsitektur OPCODE yang modular**

- **Enables imports such as `from haicode.opcode import OpcodeRegistry`**  
  -> **Memungkinkan impor seperti `from haicode.opcode import OpcodeRegistry`**

---

### ***Relation to Haicode***

**This file acts as the entry point for HOM integration.**  
-> **File ini bertindak sebagai titik masuk untuk integrasi HOM.**

**It allows Haicode grammar to access OPCODE via HOM paths.**  
-> **Memungkinkan grammar Haicode mengakses OPCODE melalui jalur HOM.**

---

## ***File 2: opcode/opcode.py***

### ***Description***

**This file defines the Master Opcode Registry.**  
-> **File ini mendefinisikan Master Opcode Registry.**

**It manages the global collection of all OPCODE definitions.**  
-> **Registry ini mengelola koleksi global seluruh OPCODE.**

**Each OPCODE includes metadata such as name, arguments, and target mapping.**  
-> **Setiap OPCODE memiliki metadata seperti nama, argumen, dan target mapping.**

---

### ***Core Structure***

**OpcodeRegistry is the central registry class.**  
-> **OpcodeRegistry adalah kelas registry pusat.**

**It stores OPCODE objects and their metadata.**  
-> **Kelas ini menyimpan objek OPCODE dan metadata-nya.**

---

### ***Key Methods***

- **register() — add new OPCODE with metadata**  
  -> **register() — menambahkan OPCODE baru dengan metadata**

- **lookup() — find OPCODE by uppercase name**  
  -> **lookup() — mencari OPCODE berdasarkan nama uppercase**

- **dispatch() — forward execution to executor**  
  -> **dispatch() — meneruskan eksekusi ke executor**

- **list_opcodes() — list all registered OPCODEs**  
  -> **list_opcodes() — menampilkan semua OPCODE terdaftar**

---

### ***Global Instance***

**A global MASTER_REGISTRY is provided.**  
-> **Disediakan instance global MASTER_REGISTRY.**

**This allows easy access from Haicode grammar and HOM.**  
-> **Hal ini memungkinkan akses mudah dari grammar Haicode dan HOM.**

---

### ***Relation to Haicode***

**This file is the semantic and operational center of OPCODE.**  
-> **File ini adalah pusat semantik dan operasional OPCODE.**

**It is comparable to CPython’s opcode.py but intent-oriented.**  
-> **Mirip dengan opcode.py di CPython, namun berorientasi intent.**

---

## ***File 3: opcode/opcode_base.py***

### ***Description***

**This file defines the base class for all OPCODE objects.**  
-> **File ini mendefinisikan base class untuk semua objek OPCODE.**

**All concrete OPCODE implementations inherit from this class.**  
-> **Semua implementasi OPCODE konkret mewarisi kelas ini.**

---

### ***Core Design***

**OpcodeBase is an abstract base class (ABC).**  
-> **OpcodeBase adalah abstract base class (ABC).**

**It enforces a consistent structure across all OPCODEs.**  
-> **Kelas ini memastikan struktur yang konsisten untuk semua OPCODE.**

---

### ***Key Methods***

- **execute() — abstract execution method**  
  -> **execute() — method abstrak untuk eksekusi**

- **__init__() — initialize metadata**  
  -> **__init__() — inisialisasi metadata**

- **get_metadata() / set_metadata() — manage metadata**  
  -> **get_metadata() / set_metadata() — mengelola metadata**

- **register() — register to master registry**  
  -> **register() — mendaftarkan ke master registry**

---

### ***Relation to Haicode***

**This class bridges semantic intent and operational execution.**  
-> **Kelas ini menjembatani intent semantik dan eksekusi operasional.**

**It ensures all OPCODEs follow the same execution contract.**  
-> **Memastikan semua OPCODE mengikuti kontrak eksekusi yang sama.**

---

## ***File 4: opcode/opcode_types.py***

### ***Description***

**This file defines OPCODE categories using enumerations.**  
-> **File ini mendefinisikan kategori OPCODE menggunakan enumerasi.**

**Each type represents a class of operations.**  
-> **Setiap tipe merepresentasikan kelas operasi tertentu.**

---

### ***Purpose***

**OPCODE types ensure semantic and operational consistency.**  
-> **Tipe OPCODE memastikan konsistensi semantik dan operasional.**

**They are used in metadata, validation, and dispatch.**  
-> **Digunakan dalam metadata, validasi, dan dispatch.**

---

### ***Examples of Types***

- **Arithmetic** → ADD, SUB, MUL, DIV  
  -> **Aritmatika → ADD, SUB, MUL, DIV**

- **IO** → PRINT, READ, WRITE  
  -> **Input/Output → PRINT, READ, WRITE**

- **AI** → TENSOR, MODEL, INFER  
  -> **AI → TENSOR, MODEL, INFER**

---

### ***Relation to Haicode***

**OpcodeType separates semantic-only and executable instructions.**  
-> **OpcodeType memisahkan instruksi semantik dan instruksi eksekusi nyata.**

---

## ***File 5: opcode/opcode_registry.py***

### ***Description***

**This file provides registration and lookup utilities for OPCODE.**  
-> **File ini menyediakan utilitas pendaftaran dan pencarian OPCODE.**

**It integrates directly with the Master Opcode Registry.**  
-> **Terintegrasi langsung dengan Master Opcode Registry.**

---

### ***Key Functions***

- **register_opcode() — register OPCODE safely**  
  -> **register_opcode() — mendaftarkan OPCODE secara aman**

- **lookup_opcode() — retrieve OPCODE by name**  
  -> **lookup_opcode() — mengambil OPCODE berdasarkan nama**

- **list_all_opcodes() — monitoring and debugging**  
  -> **list_all_opcodes() — monitoring dan debugging**

---

### ***Relation to Haicode***

**This module enables modular OPCODE loading from sets/.**  
-> **Modul ini memungkinkan pemuatan OPCODE secara modular dari sets/.**

---

## ***File 6: opcode/opcode_executor.py***

### ***Description***

**This file defines the OPCODE execution dispatcher.**  
-> **File ini mendefinisikan dispatcher eksekusi OPCODE.**

**It receives OPCODE and arguments, then routes execution.**  
-> **Menerima OPCODE dan argumen, lalu merutekan eksekusi.**

---

### ***Execution Model***

**The executor does not execute logic directly.**  
-> **Executor tidak mengeksekusi logika secara langsung.**

**It dispatches execution to the appropriate adapter.**  
-> **Ia mendispatch eksekusi ke adapter yang sesuai.**

---

### ***Key Responsibilities***

- **Dispatch OPCODE to runtime adapters**  
  -> **Mendispatch OPCODE ke adapter runtime**

- **Act as a placeholder for real execution**  
  -> **Berperan sebagai placeholder eksekusi nyata**

- **Maintain execution status**  
  -> **Menjaga status eksekusi**

---

### ***Relation to Haicode***

**This file connects semantic OPCODE to real execution targets.**  
-> **File ini menghubungkan OPCODE semantik ke target eksekusi nyata.**

**It completes the intent → goal → opcode execution chain.**  
-> **Melengkapi rantai eksekusi intent → goal → opcode.**

---

# ***Final Architectural Summary***

**OPCODE files form a complete execution backbone.**  
-> **File-file OPCODE membentuk tulang punggung eksekusi penuh.**

**They preserve semantic meaning while enabling low-level execution.**  
-> **Mereka menjaga makna semantik sambil memungkinkan eksekusi low-level.**

**This architecture is modular, extensible, and runtime-agnostic.**  
-> **Arsitektur ini modular, extensible, dan agnostik terhadap runtime.**
