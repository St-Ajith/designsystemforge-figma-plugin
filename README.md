# designsystem.build — Figma Plugin

Generate design systems from your brand directly inside Figma.

> **Note:** This plugin is currently under review on Figma Community. Until it's approved, install it manually using the steps below — it takes less than a minute.

---

## Install manually (Development mode)

### Step 1 — Download the plugin

Click the green **Code** button at the top of this page → **Download ZIP**

Or clone it:
```bash
git clone https://github.com/St-Ajith/designsystemforge-figma-plugin.git
```

### Step 2 — Import into Figma

1. Open **Figma Desktop** (the plugin won't load from the browser)
2. Go to the menu: **Figma** → **Plugins** → **Development** → **Import plugin from manifest…**
3. Navigate to the downloaded folder and select `manifest.json`
4. Click **Open**

### Step 3 — Run the plugin

1. Open any Figma file
2. Go to **Plugins** → **Development** → **designsystem.build**
3. Paste your **export token** from [design-system.up.railway.app](https://design-system.up.railway.app)
4. Click **Build Design System** — done!

---

## What the plugin generates

- 🎨 **Color variables** — Primitives + Semantic (Light & Dark), properly scoped
- **Text styles** — Display, Heading, Body, Label, Code using your brand fonts  
- 🎨 **Color styles** — Every semantic token + shade scale in the Styles panel
- 🧩 **Component sets** — Real Figma components with variant properties + token bindings

---

## Troubleshooting

**"Cannot import plugin from browser"**  
You need Figma Desktop, not the web version. [Download it here](https://www.figma.com/downloads/).

**"Plugin not showing up"**  
Make sure you selected `manifest.json` (not from inside a subfolder).

**"Invalid token"**  
Tokens expire after 1 hour. Go back to the Export tab and generate a new one.

---

## Files

| File | Description |
|------|-------------|
| `manifest.json` | Plugin metadata — required by Figma |
| `code.js` | Plugin logic (runs in Figma sandbox) |
| `ui.html` | Plugin UI panel |

---

Once approved: [Figma Community](https://www.figma.com/community/plugin/1623830472453970738)

Built with ❤️ by [designsystem.build](https://design-system.up.railway.app) · [LinkedIn](https://www.linkedin.com/in/ajith-kumar-v/)

---

## Changelog

### v1.4.0 — April 2026
- **Light + Dark side-by-side** — Variants section now renders both Light and Dark mode cards next to each other. No more mode-toggling in the Variables panel — see both themes at a glance.
- **Real Figma variable modes** — `Semantic/Colors` and `Component/Tokens` collections now have proper Light and Dark modes. Switching the collection mode in Figma updates all token-bound colours automatically.
- **Custom colour overrides flow to Figma** — Colours customised in the web app (via the Customise editor) are now exported as real Figma variables in the correct mode (Light or Dark).

### v1.3.0
- Button spec v2: Danger variant, icon-only sizes, per-variant colour customisation
- Font size corrections: SM=14px, MD=16px, LG=18px

### v1.2.0
- All 25 component anatomy handlers implemented
- Snackbar, tag, input, list, radio, tooltip shapes rebuilt from scratch
- ComponentSet (purple dashed border) for all variant grids

---
