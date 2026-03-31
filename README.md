Crimson Desert Shop Editor




1. Get the required tools
2. 
Download a PAZ unpacker:

[Crimson Desert Unpacker](https://www.nexusmods.com/crimsondesert/mods/62)

[Crimson Browser](https://www.nexusmods.com/crimsondesert/mods/84)

You need one of these to extract game files.

4. Extract the required game files

Using the unpacker, go into the game’s data files and extract:

iteminfo.pabgb → contains all item IDs and names
storeinfo.pabgb → contains all shop inventories (slots + stock)

These are usually found in something like gamedata/

3. Load your files into the editor

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
4. Load localization
Select a language from the dropdown (e.g. English)
Without this you’ll see raw/internal item names

5. Browse and select a shop
Use the left sidebar
Stores are grouped by city/region
Click a store to open it

You’ll now see:
All slots in that shop
Each slot = 1 item the shop sells

6. Understand shop slots

Each slot shows:

Item name
Item hex ID
Stock value (editable)
Slot number

Example:

Slot 1 → Iron Sword
Stock: 50

7. Modify Stock
Each slot has a stock input field
You can change it directly

Minimum: 1
Maximum: 9999

When you change stock:

The slot is marked as modified

8. Change Items
Click a slot (left panel)
Search for an item (right panel)
Click Assign →

This will replace the item in that slot
Keep or apply the current stock value

9. Search for items

Use the search box:

By name
By internal name
By hex ID

10. Make multiple edits

You can:
Change multiple slots
Change stock only
Change item + stock

All changes are tracked as: MODIFIED

11. Export your mod

Export JSON Button

This generates your mod data with:

New item assignments
New stock values
Metadata (name, author, version)

12. Customize mod info (bottom bar)

You can edit:

Mod Name
Author
Version

This is included in the export.

13. Reset if needed

Click:

Reset

This clears all changes for the current store.

14. Use JSON Mod Manager to load your Json
[JSON Mod Manager](https://www.nexusmods.com/crimsondesert/mods/113)
