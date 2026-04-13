# designsystem.build Figma Plugin — Changelog

## v1.4.0 — April 2026

### ✨ New: Light + Dark side-by-side variant grid
Each component's **Variants** section now shows two panels side by side:
- ☀ **Light panel** — white background, using Light variable mode
- 🌙 **Dark panel** — dark background, using Dark variable mode

Designers can see both themes simultaneously without toggling Figma's variable modes panel.

### ✨ New: Real Light + Dark Figma variable modes
- `Semantic/Colors` collection now creates genuine **Light** and **Dark** modes
- `Component/Tokens` collection also has **Light** and **Dark** modes
- Per-component colour overrides from the web editor (e.g. custom badge colours) flow into the correct mode in Figma variables

### ✨ New: Custom colour overrides in Figma
Colours you customise in the web editor (via the **Customise** drawer on any component page) are now exported as Figma variables with both light and dark values. Change a badge's error colour → export → it appears in the `Component/Tokens` collection with your custom value.

---

## v1.3.0 — March 2026

### ✨ New: Danger/Destructive button variant
- Added `danger` variant to the Button component
- Renders with error colour background and white text

### Fix: Button font sizes
- SM: 14px, MD: 16px, LG: 18px (was 12/13/15)

---

## v1.2.0 — February 2026

### ✨ New: Button spec v2
- 6 variants: primary, secondary, tertiary, ghost, link, danger
- Icon-only sizes: SM=40×40, MD=44×44, LG=48×48 (min 44px touch target)
- All button sizes comply with WCAG 2.5.5 Target Size

---

## Installing the plugin

Until the plugin is approved on Figma Community, install manually:

1. Clone or download this repo
2. Open Figma Desktop → Plugins → Development → Import plugin from manifest
3. Select `manifest.json` from this folder
4. The plugin will appear under **Plugins → Development → designsystem.build**
