Crimson Desert Shop Editor




1. Get the required tools
Download a PAZ unpacker (example):
https://www.nexusmods.com/crimsondesert/mods/62
You need this to extract game files.
2. Extract the required game files

Using the unpacker, go into the game’s data files and extract:

iteminfo.pabgb → contains all item IDs and names
storeinfo.pabgb → contains all shop inventories (slots + stock)

These are usually found in something like:

gamedata/
3. Open the Shop Editor
Open the index.html file in your browser
You’ll see the editor UI load
4. Load your files into the editor

On the left side:

📦 Load item database
Click iteminfo.pabgb
This enables the item browser
🏪 Load store data
Click storeinfo.pabgb
This enables store editing

✔ Once both are loaded:

Stores appear in the sidebar
Items appear in the item browser
5. (Optional but recommended) Load localization
Select a language from the dropdown (e.g. English)
This replaces internal names with real item names

Without this:

You’ll see raw/internal item names
6. Browse and select a shop
Use the left sidebar
Stores are grouped by city/region
Click a store to open it

You’ll now see:

All slots in that shop
Each slot = 1 item the shop sells
7. Understand shop slots

Each slot shows:

Item name
Item hex ID
Stock value (editable)
Slot number

Example:

Slot 1 → Iron Sword
Stock: 50
8. Modify stock (NEW FEATURE)
Each slot has a stock input field
You can change it directly

✔ Rules:

Minimum: 1
Maximum: 9999 (UI allows this even if you said 100 earlier)

When you change stock:

The slot is marked as modified
9. Change items in a slot
Click a slot (left panel)
Search for an item (right panel)
Click Assign →

✔ This will:

Replace the item in that slot
Keep or apply the current stock value
10. Search for items

Use the search box:

By name
By internal name
By hex ID
11. Make multiple edits

You can:

Change multiple slots
Change stock only
Change item + stock

All changes are tracked as:

MODIFIED
12. Export your mod

Click:

Export JSON

This generates your mod data with:

New item assignments
New stock values
Metadata (name, author, version)
13. Customize mod info (bottom bar)

You can edit:

Mod Name
Author
Version

This is included in the export.

14. Reset if needed

Click:

Reset

This clears all changes for the current store.

15. Use JSON Mod Manager to load your Json
https://www.nexusmods.com/crimsondesert/mods/113
