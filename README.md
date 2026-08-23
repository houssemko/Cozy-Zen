---

# 🌿 Cozy-Zen

My personal, tweaked CSS theme for the [Zen Browser](https://zen-browser.app/) — Zen Browser with quality of life improvements centered around the Compact Sidebar.

## 📦 Included Mods

The theme is organized as a set of small, focused CSS modules, each targeting a specific part of the UI:

| Module | Purpose |
| ------ | ------- |
| `Sidebar.css` | Compact sidebar styling and behavior |
| `TabStyles.css` | Tab appearance tweaks |
| `TabGroups.css` | Tab group styling |
| `URLbar.css` | Address bar styling |
| `Findbar.css` | Find / search bar styling |
| `Context-Menu.css` | Context menu styling |
| `Window-Buttons.css` | Window control buttons |
| `Animations.css` | UI animations and transitions |
| `CMI/` | [Context-Menu-Icons](#-context-menu-icons-cmi) — icon pack for context menus |

### ✨ Context-Menu-Icons (CMI)
[Context-Menu-Icons](https://github.com/Starry-AXQG/Context-Menu-Icons) adds beautiful FluentUI/ZenUI icons to all context menus — including tabs, bookmarks, extensions and zenFolders. It ships with two icon sets (`FluentUI/` and `ZenUI/`) plus `global.css`, `preferences.css` and the `CMI-config.css` customization file.

### 🎨 Content Styling
- `betterpdf.css` — improves the built-in PDF viewer.
- `compact-settings.css` — compacts the `about:preferences` / `about:settings` pages.

> **Note**: Content styles are applied via `userContent.css`. Update it to `@import` whichever of the files under `content/` you want active.

---

## 🛠️ Installation

### 1. Set Up Your `chrome` Folder
If you haven’t already, enable `userChrome.css` support in Zen:
- Go to `about:config`
- Set `toolkit.legacyUserProfileCustomizations.stylesheets` to `true`
- Locate your [Zen profile folder](https://docs.zen-browser.app/guides/live-editing) and create a `chrome` folder inside it.

### 2. Install Cozy-Zen
1. Download or clone this repo.
2. Copy the entire contents of this repository into your `chrome` folder:
   ```
   [Your Zen Profile]/
   └── chrome/
       ├── userChrome.css        ← main stylesheet (imports modules/)
       ├── userContent.css       ← content / page styling (imports content/)
       ├── content/              ← page-level styles
       │   ├── betterpdf.css
       │   └── compact-settings.css
       ├── user.js
       └── modules/              ← organized mod directory
           ├── Animations.css
           ├── Context-Menu.css
           ├── Findbar.css
           ├── Sidebar.css
           ├── TabGroups.css
           ├── TabStyles.css
           ├── URLbar.css
           ├── Window-Buttons.css
           └── CMI/              ← Context-Menu-Icons (CMI)
               ├── CMI-config.css   ← ✅ customization file (edit this!)
               ├── global.css
               ├── preferences.css
               ├── FluentUI/        ← FluentUI icon set
               └── ZenUI/           ← ZenUI icon set
   ```

> 💡 **Important**: The `CMI-config.css` file **must remain inside** the `CMI/` folder for CMI to load properly.

### 3. Enable Required Preference
In `about:config`, ensure this setting is **enabled**:
```
svg.context-properties.content.enabled = true
```
> ⚠️ CMI will **not run** without this.

### 4. Place `user.js`
Place `user.js` inside your [Zen profile folder], or add its contents to the end of an existing `user.js` file.

### 5. Restart Zen Browser
After copying files and setting preferences, fully restart Zen to apply changes.


---

## 🔄 Updating CMI

Since CMI updates frequently:
1. Download the latest release from [Starry-AXQG/Context-Menu-Icons](https://github.com/Starry-AXQG/Context-Menu-Icons)
2. Preserve your customizations by re-applying them to `CMI-config.css`, or replace it with your previous one.
3. Replace the contents of your `modules/CMI/` folder with the new `CMI/` folder.

> 🔜 *(Future note: Consider using [Sine](https://sine.zen-browser.app/) for auto-updates—but manual install gives full control.)*

---

## 🙏 Credits
 
- **[Zen Browser](https://zen-browser.app/)** – The beautiful, Firefox-based browser that makes this possible  
- **[Context-Menu-Icons](https://github.com/Starry-AXQG/Context-Menu-Icons)** by [Starry-AXQG](https://github.com/Starry-AXQG) 
- **[Arc-2.0](https://github.com/YashjitPal/Arc-2.0)** by [YashjitPal](https://github.com/YashjitPal)  
- **[bubble-clean-zen](https://github.com/nieffka/bubble-clean-zen)** by [nieffka](https://github.com/nieffka)

---

## 📝 License

This theme is licensed under the [MIT License](LICENSE). Respect the licenses of all included mods.  
CMI is licensed under its own terms—see its [repository](https://github.com/Starry-AXQG/Context-Menu-Icons) for details.

---
