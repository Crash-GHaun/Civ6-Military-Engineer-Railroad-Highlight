# Military Engineer Railroad Highlight (Civ VI)

A lightweight UI mod for **Civilization VI: Gathering Storm** that provides a live map overlay for your railroad network.

## The Problem
In the late game, it is notoriously difficult to see where your railroad network is complete and where gaps remain, especially on certain terrain types or with high-density districts.

## The Solution
When a **Military Engineer** is selected, the mod automatically highlights every tile containing a railroad that is visible to you. 

* **Automatic:** Highlights appear on selection and disappear on deselection.
* **Live:** Updates immediately as you build or as tiles are pillaged.
* **Compatible:** Uses the "Great People" lens layer to ensure it doesn't flicker or conflict with major UI overhauls like *More Lenses* or *CUI*.

## Installation

### Steam Workshop
The easiest way to install is via the [Steam Workshop](https://steamcommunity.com/sharedfiles/filedetails/?id=3724416742).

### Manual Installation (GitHub)
If you prefer a manual install:
1. Download the repository as a ZIP.
2. Extract the folder to your Civ VI Mods directory:
    * **Windows:** `Documents\My Games\Sid Meier's Civilization VI\Mods\`
    * **Linux:** `~/.local/share/aspyr-media/Sid Meier's Civilization VI/Mods/`
3. Enable "Military Engineer Railroad Highlight" in the **Additional Content** menu in-game.

## Technical Details
The mod is written in Lua and utilizes the game's native `UILens` API. It hooks into `UnitSelectionChanged` and `RouteChanged` events to ensure the overlay is always accurate without impacting game performance.

By using the `Hex_Coloring_Great_People` layer, the mod ensures that it doesn't fight for control over the lens system with other popular mods that might be monitoring the Religion or Appeal lenses.

---
**Created by crash**