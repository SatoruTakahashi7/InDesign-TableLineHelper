# InDesign TableLineHelper

`TableLineHelper.jsx`  
Japanese name: `表組の罫線をいじるやつ.jsx`

An InDesign script that helps you edit table cell borders/strokes.

Select table cells, run the script, and use a clearer, easier-to-click UI for applying table strokes.  
This tool is intended to make common table border operations more practical than using InDesign’s standard Stroke panel alone.

---

## Features

- Manual launch after selecting table cells
- Apply all borders
- Apply outer borders
- Apply inner borders
- Clear outer borders
- Clear inner borders
- Clear all borders
- Apply thick outer borders + thin inner borders
- Individually select:
  - Top
  - Bottom
  - Left
  - Right
  - Inner horizontal
  - Inner vertical
- Visual border selection UI
- Manual stroke weight input and preset weight selection
- Supports `mm` and `pt`
- Stroke style dropdown
- Swatch color dropdown
- Remembers previous settings
- User-defined presets: save / load / delete
- Automatically applies preset settings to the UI when selected
- Warning dialog when using inner-border operations on merged cells
- Experimental numeric keypad support for border selection

---

## Changelog

### v0.9.3

- Added user-defined presets.
- Presets now automatically update the UI when selected.
- Added experimental numeric keypad support for border selection.
- Unified Quick Operation and Line Selection under a single `Run` button.
- Improved the visual border selection UI.

### v0.9.1

- Fixed an issue where stroke tint could become blank when `Apply color and stroke style` was enabled.
- Stroke tint is now set to 100% when color and stroke style are applied.

### v0.9.0

- Initial public release.

---

## Usage

1. Select table cells in InDesign.
2. Run `TableLineHelper.jsx` from the Scripts panel.
3. Choose a processing mode:
   - Quick Operation
   - Line Selection
4. Set the stroke weight, unit, and optionally color/stroke style.
5. Click the `Run` button to apply the stroke settings.

---

## Quick Operations

The following quick operations are available:

- Apply all borders
- Apply outer borders
- Apply inner borders
- Clear outer borders
- Clear inner borders
- Clear all borders
- Apply thick outer borders + thin inner borders

---

## Line Selection

In Line Selection mode, you can select individual borders:

- Top
- Bottom
- Left
- Right
- Inner horizontal
- Inner vertical

You can also click the visual border selection UI to choose the target borders.

---

## Numeric Keypad Shortcuts  
Experimental feature

Numeric keypad shortcuts can be used to toggle border selections.

- `7`: Top + Left
- `8`: Top
- `9`: Top + Right
- `4`: Left
- `5`: Inner horizontal + Inner vertical
- `6`: Right
- `1`: Bottom + Left
- `2`: Bottom
- `3`: Bottom + Right
- `0`: Clear all selections
- `.`: Select all borders

Numeric keypad support is experimental.  
Depending on your keyboard, operating system, InDesign version, or ScriptUI focus state, it may not work as expected.

---

## Presets

You can save the current UI state as a preset.

Presets can store settings such as:

- Stroke weight
- Unit
- Whether color/stroke style should be applied
- Stroke style
- Swatch color
- Processing mode
- Quick operation
- Line selection state
- Outer/inner stroke weights for thick outer + thin inner operations

When a preset is selected, the saved settings are automatically applied to the UI.  
Check the displayed settings, then click `Run` to apply them.

---

## Installation

Place `TableLineHelper.jsx` in InDesign’s `Scripts Panel` folder.

Example path on macOS:

```text
~/Library/Preferences/Adobe InDesign/Version XX.X/en_US/Scripts/Scripts Panel/
