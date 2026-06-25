# FloatingCheckbox

FloatingCheckbox

A PowerApps Component Framework (PCF) control that renders a Dataverse multiselect choice (option set) field as a row of pill-shaped, tappable buttons — instead of the default dropdown/checklist UI.

<img width="373" height="112" alt="image" src="https://github.com/user-attachments/assets/c6f24528-88aa-4a77-8600-282b73253f53" />


Why use this control?

The out-of-the-box multiselect option set control in model-driven apps renders as a small dropdown with checkboxes, which:


Hides all options behind a click before the user can even see what's available
Doesn't scale well visually when there are many options
Gives no styling flexibility to match brand colors or visual hierarchy


FloatingCheckbox instead shows every option as a standalone pill button, all visible at once, with selected options visually highlighted. Users toggle selections with a single click — no dropdown, no extra step.

Features


Works with any Dataverse multiselect choice (option set) field — not tied to a specific entity or set of options
Fully configurable styling: font family, font size, selected color, unselected color, and text color
Sensible defaults applied automatically if no styling values are configured
Instant visual feedback on click (no waiting for form refresh)
Lightweight — no external UI framework dependencies

Configurable properties

PropertyTypeRequiredDefaultDescriptionchoicesFieldMultiSelectOptionSetYes—The multiselect choice field to bind. This is set automatically when added to a field.fontFamilyTextNoSegoe UIFont family applied to the pill labels.fontSizeWhole NumberNo13Font size (in pixels) for the pill labels.selectedColorText (hex color)No#1c3f94Background/border color for a selected pill. Must be a valid hex code (e.g. #1c3f94 or #fff).unselectedColorText (hex color)No#ffffffBackground color for an unselected pill.textColorText (hex color)No#1f2d4dText color for unselected pill labels. Selected pills always use white text for contrast.

Note on color properties: if a value is left blank, or isn't a valid hex color, the control automatically falls back to its default — invalid input never breaks rendering.
