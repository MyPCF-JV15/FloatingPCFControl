# FloatingCheckbox

FloatingCheckbox

A PowerApps Component Framework (PCF) control that renders a Dataverse **multiselect choice (option set)** field as a row of pill-shaped, tappable buttons — instead of the default dropdown/checklist UI.

<img width="373" height="112" alt="image" src="https://github.com/user-attachments/assets/c6f24528-88aa-4a77-8600-282b73253f53" />


## Why use this control?
 
The out-of-the-box multiselect option set control in model-driven apps renders as a small dropdown with checkboxes, which:
- Hides all options behind a click before the user can even see what's available
- Doesn't scale well visually when there are many options
- Gives no styling flexibility to match brand colors or visual hierarchy

**FloatingCheckbox** instead shows every option as a standalone pill button, all visible at once, with selected options visually highlighted. Users toggle selections with a single click — no dropdown, no extra step.

## Features
 
- Works with **any** Dataverse multiselect choice (option set) field — not tied to a specific entity or set of options
- Fully configurable styling: font family, font size, selected color, unselected color, and text color
- Sensible defaults applied automatically if no styling values are configured
- Instant visual feedback on click (no waiting for form refresh)
- Lightweight — no external UI framework dependencies


## Configurable properties

When you add FloatingCheckbox to a field, the form editor's property panel shows one required field-binding property and five optional styling properties:
 
| Property | Type | Required | Default | Description |
|---|---|---|---|---|
| **Choices Field** | MultiSelectOptionSet | Yes | — | The multiselect choice field to bind. Set automatically — this is the field you attached the control to. |
| **Font Family** | Text | No | `Segoe UI` | Font family applied to the pill labels. |
| **Font Size** | Whole Number | No | `13` | Font size (in pixels) for the pill labels. |
| **Selected Color** | Text (hex color) | No | `#1c3f94` | Background/border color for a selected pill. Must be a valid hex code (e.g. `#1c3f94` or `#fff`). |
| **Unselected Color** | Text (hex color) | No | `#ffffff` | Background color for an unselected pill. |
| **Text Color** | Text (hex color) | No | `#1f2d4d` | Text color for unselected pill labels. Selected pills always use white text for contrast. |
 <img width="106" height="300" alt="image" src="https://github.com/user-attachments/assets/1b9bf25f-680f-4b3f-b0c8-877c00f1cb56" />

Note on color properties: if a value is left blank, or isn't a valid hex color, the control automatically falls back to its default — invalid input never breaks rendering.
