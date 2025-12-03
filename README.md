A lightweight, browser-based XML loadout editor designed for FiveM-style agency vehicle configurations.  
Uses **pure text-based, lossless parsing** to ensure your original XML formatting is preserved exactly.

---
<img width="2516" height="1106" alt="image" src="https://github.com/user-attachments/assets/0164c468-d4cd-4fe6-afcf-c0fca5618471" />

## ✨ Features

### 🔒 Lossless XML Editing
- Parses XML as raw text (no DOM rewriting)
- Preserves:
  - indentation  
  - whitespace  
  - original line ordering  
  - comments  
- Only modifies the contents between `<Vehicles>` and `</Vehicles>`

### 🚔 Vehicle Editing UI
- Edit vehicle names  
- Change or remove `chance=""` values  
- Delete vehicles  
- Add new vehicle entries  
- “Boost” button increases chance by +20  

- **Equalize** evenly distributes chance values across all vehicles

### 📦 Preset Vehicle Library
- Preloaded with large sets of:
  - LSPD  
  - LSSD  
  - BCSO  
  - SAHP  
  - Ranger  
  - SASPA  
  - NOOSE  
  - USAF  
  - Port Authority  
  - Rockford Hills PD  
  - Airport (LSIA)  
- Fully grouped + collapsible modal UI  
- 1-click insertion into any loadout

### 📥 Bulk Add Tool
- Paste multiple vehicle names (one per line)
- Instantly inserts all with `chance="0"`  
- Useful for mass imports or migrating packs

### 💾 Export System
- Outputs the modified XML with all formatting intact  
- Only replaces `<Vehicle>` entries inside `<Vehicles>` blocks  
- Never modifies unrelated XML

---

## 📘 How to Use

1. Paste your XML into the **Input XML** box  
2. Click **Parse XML**  
3. Scroll to the agency + loadout you want to edit  
4. Use:
   - Add Vehicle  
   - Equalize  
   - Add Preset  
   - Bulk Add  
5. Click **Generate XML**  
6. Copy paste the new lossless XML

---

## 🧪 Known Limitations
- Only supports `<Vehicles>` inside `<Loadout>` blocks  
- Ignores all `<Vehicles>` outside the editable structure  
- Loadouts must contain exactly one `<Name>` tag  
- Does not validate XML correctness  
- Chance equalization does not enforce total = 100 (by design)

---

## 🛠 Version
`v0.1 — Early Prototype`

Future versions will include:
- preset search bar  
- sorting  
- drag-to-reorder vehicles  
- multiple loadout editors  
- XML validator  
- full DOM diff mode  
