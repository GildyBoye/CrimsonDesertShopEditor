# Crimson Desert Shop Editor

A browser-based tool for editing shop inventories in Crimson Desert. Change what items vendors sell, adjust stock quantities, and export a JSON mod file ready to load with the JSON Mod Manager.

> 🔗 Join the community: [Discord](https://discord.gg/mQjgHCW)
> Video Start: https://www.youtube.com/watch?v=vPr9knDL1sw

---

## Quick Start — No Tools Required

If you just want to get started immediately, click **"Use pre-built base files (v1.01.02)"** in the editor.

This loads pre-extracted versions of the required game files directly — no unpacker needed. Keep in mind these base files reflect a specific game version and may fall behind after updates. When that happens, extract and upload your own files for the most accurate data.

---

## Full Setup — Using Your Own Game Files

For the most up-to-date data, extract the files yourself using a PAZ unpacker.

**Step 1 — Get an unpacker**

You need one of these tools to extract files from the game's data archives:

- [Crimson Desert Unpacker](https://www.nexusmods.com/crimsondesert/mods/62)
- [Crimson Browser](https://www.nexusmods.com/crimsondesert/mods/84)

**Step 2 — Extract the required files**

Using your unpacker, locate and extract from `gamedata/`:

- `iteminfo.pabgb` — all item IDs and names
- `storeinfo.pabgb` — all shop inventories (slots and stock values)

**Step 3 — Load your files into the editor**

On the left sidebar:

- 📦 Click the **iteminfo.pabgb** drop zone and select your extracted file
- 🏪 Click the **storeinfo.pabgb** drop zone and select your extracted file

Once both are loaded, the store list and item browser will populate automatically.

---

## Using the Editor

**Localization**

Select a language from the dropdown (e.g. English). This is loaded automatically on startup. Without it you'll see raw internal item names instead of proper display names.

**Browsing stores**

Stores are listed in the left sidebar, grouped by city or region. Click any city header to expand it, then click a store to open it. You can also use the search box to find a store by name.

**Understanding slots**

Each slot in a store represents one item that vendor sells. Every slot shows:
- Item name (or hex ID if the item is unresolvable)
- Stock quantity (editable directly)
- Slot number

**Modifying stock**

Each slot has a stock input you can edit directly. Valid range is 1–9999. Changing stock alone marks the slot as modified without requiring an item swap.

**Changing items**

1. Click a slot in the left panel to select it
2. Browse or search for an item in the right panel
3. Click **Assign →** to replace the item in that slot

Items are sorted into categories (Armor, Weapons, Food, etc.) and all collapsed by default. Use the search box to find items by name, internal name, or hex ID.

**Unknown items**

Some slots contain items the editor cannot identify — these show as `Unknown Item (XXXXXX)`. If you try to assign one of these, you'll be asked to confirm, as they may be important to the store's function.

**Making multiple edits**

You can modify as many slots as you like before exporting. All changed slots are highlighted as **MODIFIED**. Switching to a different store resets any unsaved changes for the current one.

**Exporting your mod**

Click **Export JSON** in the top toolbar. This downloads a `.json` file containing your changes — new item assignments, stock values, and metadata. Load this file with the JSON Mod Manager.

**Resetting changes**

Click **Reset** to clear all modifications for the current store and start fresh.

---

## Loading Your Mod In-Game

Use the [JSON Mod Manager](https://www.nexusmods.com/crimsondesert/mods/113) to load the exported `.json` file.

---

> ⚠️ **Back up your saves before modifying your game.**

---

*All game files and assets belong to Pearl Abyss. This tool is a fan-made utility — buy the game and support the developers!*
