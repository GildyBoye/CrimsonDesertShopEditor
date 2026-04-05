# Crimson Desert Modding Toolkit

A browser-based multi-editor for modifying game data in **Crimson Desert**.  
Edit shop inventories, trust/drop values, skills, and item prices — then export ready-to-use JSON mods.

> 🔗 Join the community: [Discord](https://discord.gg/mQjgHCW)  
> 🎥 Video Start: https://www.youtube.com/watch?v=vPr9knDL1sw  

---

## Overview

This tool includes **four editors in one UI**:

- 🏪 **Shop Editor** — modify store inventories & stock
- 🤝 **Dropset Editor** — edit trust gain / drop-related values
- ⚔️ **Skill Editor** — patch skill data via hex edits
- 💰 **Price Editor** — change item buy prices

Switch between them using the dropdown in the top-left of the app.

---

## Quick Start — No Tools Required

If you just want to jump in:

- Click **"Use pre-built base files"** (available in Shop + Price editors)

This loads pre-extracted data directly into the app.

⚠️ These are tied to a specific game version and may become outdated after patches.

---

## Full Setup — Using Your Own Game Files

For accurate and up-to-date data:

### Step 1 — Get an unpacker

Use one of these:

- [Crimson Desert Unpacker](https://www.nexusmods.com/crimsondesert/mods/62)  
- [Crimson Browser](https://www.nexusmods.com/crimsondesert/mods/84)

---

### Step 2 — Extract required files

From `gamedata/`, extract:

| Editor | Required File |
|--------|-------------|
| Shop Editor | `iteminfo.pabgb`, `storeinfo.pabgb` |
| Dropset Editor | `dropsetinfo.pabgb` |
| Skill Editor | `skill.pabgb` |
| Price Editor | `iteminfo.pabgb` (optional but recommended) |

---

### Step 3 — Load files into the editor

Each editor has its own **file drop zone** in the sidebar:

- Click or drag files into the correct slot
- Status indicators at the bottom confirm when files are loaded

---

## Shop Editor (Store Inventory Editing)

### Features

- Browse stores grouped by **city/region**
- View and edit **individual item slots**
- Modify:
  - Item assignment
  - Stock quantity (inline editable)
- Full **item browser with search + categories**
- Localization support (for proper item names)

---

### Using the Shop Editor

**1. Load required files**
- `iteminfo.pabgb`
- `storeinfo.pabgb`

**2. (Optional) Load localization**
- Select a language from the dropdown

**3. Select a store**
- Expand a region → click a store

**4. Edit slots**
- Click a slot to select it
- Change:
  - Item → via **Assign**
  - Stock → edit number directly

**5. Export**
- Click **Export JSON**

---

### Slot Behavior

- **Modified slots** are highlighted
- Stock edits alone count as a modification
- Switching stores resets unsaved changes

---

### Unknown Items

Assigning over these should trigger a confirmation — they may be important.

---

## Dropset Editor (Trust / Drop Values)

### Features

- Browse raw entries from `dropsetinfo.pabgb`
- View **hex data**
- Add manual **byte patches**
- Export patch-based JSON mods

---

### Using It

1. Load `dropsetinfo.pabgb`
2. Select an entry
3. Add patches:
   - Offset
   - Original hex
   - New hex
4. Export JSON

---

## Skill Editor

### Features

- Browse skill records
- Inspect raw binary data
- Apply hex patches per skill
- Export JSON patch mods

---

### Using It

Same workflow as Dropset Editor:

1. Load `skill.pabgb`
2. Select a skill
3. Add patches
4. Export JSON

---

## Price Editor

### Features

- Browse all items
- Modify buy price
- Automatic **copper → silver preview**
- Patch queue system
- Quick preset values

---

### Using It

1. Load:
   - Prebuilt price list **or**
   - `iteminfo.pabgb`
2. Select an item
3. Enter new price (in copper)
4. Click **Set Price**
5. Export JSON

---

## JSON Export

All editors export a **JSON patch file** containing:

- Modified values only
- Required metadata (mod name, etc.)

Use with a JSON mod loader.

---

## Mod Name

Each editor includes a **Mod Name field** — this is embedded in the exported JSON.

---

## UI Behavior Notes

- Changes are **not saved automatically**
- Store edits are **session-based**
- Status bar shows:
  - File load states
  - Current editor status
- Toast notifications confirm actions (export, load, etc.)

---

## Navigation

Use the dropdown at the top-left:

- Shop Editor
- Dropset Editor
- Skill Editor
- Price Editor

---


## Loading Your Mod In-Game

Use the [JSON Mod Manager](https://www.nexusmods.com/crimsondesert/mods/113) to load the exported `.json` file.

---

> ---

## ⚠️ Important

- Always **back up your saves**
- Game updates may break offsets or base data
- Unknown values may affect game stability

---

---

*All game files and assets belong to Pearl Abyss. This tool is a fan-made utility — buy the game and support the developers!*
