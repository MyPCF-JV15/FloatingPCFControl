# FloatingCheckbox

A PowerApps Component Framework (PCF) control that renders a Dataverse multiselect choice (option set) field as a row of pill-shaped, tappable buttons — instead of the default dropdown/checklist UI.



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
