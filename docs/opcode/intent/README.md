# Haicode Intent OPCODE Structure 
 
## Overview 
This directory (`opcode/intent/`) is a placeholder for intent-related components in Haicode's OPCODE system. It supports the intent-oriented execution model, where **lowercase words** represent **intent** (semantic triggers for meaning), **capitalized words** represent **goal** (high-level objectives), and **uppercase words** represent **opcode** (actual execution instructions). This structure ensures semantic clarity and operational efficiency, aligning with Haicode's grammar rules from v0.1 to v0.4. 
 
## Intent Semantic Rules 
Based on Haicode's grammar: 
- **Lowercase Word**: Intent (meaning/maksud) - Represents semantic triggers for natural language processing. Examples: "cetak" (print intent), "jumlah" (add intent). 
- **Capitalized Word**: Goal (tujuan) - Represents high-level objectives. Examples: "Definisikan" (define goal), "Jika" (if goal). 
- **Uppercase Word**: Opcode (eksekusi nyata) - Represents actual machine instructions. Examples: "PRINT", "ADD", "Cetak". 
 
This follows semantic rules from controlled natural language programming, where intent drives goal, and goal triggers opcode.
[pypi.org](https://pypi.org/project/intentlang/0.2.7/)
 
## Structure 
- **Purpose**: Store intent definitions, mappings, and documentation for intent-to-opcode resolution. 
- **Current Status**: Empty (struktur saja) - Intended for future expansion with intent files (e.g., intent_map.py, semantic_rules.py). 
- **Integration**: Links to Haicode grammar v0.1-v0.4 for intent parsing and execution dispatch. 
 
## Usage 
To use: 
1. Add intent files to this directory (e.g., for new intent triggers). 
2. Register intents in `opcode/registry.py` for semantic resolution. 
3. Test with Haicode programs: `Definisikan "data" kedalam (path) [ai].` 
 
## Examples from Haicode Grammar 
From v0.1-v0.4: 
- Intent: "cetak" (lowercase) → Goal: "Cetak" → Opcode: "PRINT". 
- Intent: "jumlah" (lowercase) → Goal: "Jumlah" → Opcode: "ADD". 
 
This structure enables universal instruction sets across languages, from intent to opcode.
[stackoverflow.com](https://stackoverflow.com/questions/18762446/x86-jmp-opcode-structure)
 
## Contributing 
- Add intent files for new triggers. 
- Update rules for v0.5+ grammar. 
- Test with Haicode executor. 
 
For more details, see Haicode documentation.
