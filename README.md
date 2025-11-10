---

# 🌿 Cozy-Zen

My personal, hand-crafted CSS theme for the [Zen Browser](https://zen-browser.app/), Basically Zen Browser with quality of life improvements centered around the Compact Sidebar.

## 📦 Included Mods

### ✨ [Context-Menu-Icons (CMI)](https://github.com/Starry-AXQG/Context-Menu-Icons)
> Adds beautiful FluentUI/ZenUI icons to all context menus — including tabs, bookmarks, extensions, zenFolders, and zenWorkspaces.  
- **Icon Packs**: FluentUI (default) or ZenUI
  
---

## 🛠️ Installation

### 1. Set Up Your `chrome` Folder
If you haven’t already, enable `userChrome.css` support in Zen:
- Go to `about:config`
- Set `toolkit.legacyUserProfileCustomizations.stylesheets` to `true`
- Locate your [Zen profile folder](https://github.com/zen-browser/zen/wiki/Profile-Directory) and create a `chrome` folder inside it.

### 2. Install Cozy-Zen
1. Download or clone this repo.
2. Copy the entire contents of this repository into your `chrome` folder:
   ```
   [Your Zen Profile]/
   └── chrome/
       ├── userChrome.css          ← main entry point
       ├── userContent.css
       ├── content/
       ├   └── Better-pdf.css  
       └── modules/                ← organized mod directory
           └── icons/              ← Context-Menu-Icons (CMI)
               ├── icons.css
               └──  CMI-config.css  ← ✅ customization file (edit this!)
   ```

> 💡 **Important**: The `CMI-config.css` file **must be inside** the `icons/` folder for CMI to load properly.

### 3. Enable Required Preference
In `about:config`, ensure this setting is **enabled**:
```
svg.context-properties.content.enabled = true
```
> ⚠️ CMI will **not run** without this.

### 4. Place `user.js` inside your [Zen profile folder]
### 5. Restart Zen Browser
After copying files and setting preferences, fully restart Zen to apply changes.


---

## 🔄 Updating CMI

Since CMI updates frequently:
1. Download the latest release from [Starry-AXQG/Context-Menu-Icons](https://github.com/Starry-AXQG/Context-Menu-Icons)
2. Replace the contents of your `modules/icons/` folder with the new `icons/` folder
3. Preserve your customizations by re-applying changes to `CMI-config.css` if needed

> 🔜 *(Future note: Consider using [Sine](https://sine.zen-browser.app/) for auto-updates—but manual install gives full control.)*

---

## 🙏 Credits

- **[Context-Menu-Icons](https://github.com/Starry-AXQG/Context-Menu-Icons)** by [Starry-AXQG](https://github.com/Starry-AXQG)  
- **[Zen Browser](https://zen-browser.app/)** – The beautiful, Firefox-based browser that makes this possible  
- **[Arc-2.0](https://github.com/YashjitPal/Arc-2.0)** by [YashjitPal](https://github.com/YashjitPal)  
- **[bubble-clean-zen](https://github.com/nieffka/bubble-clean-zen)** by [nieffka](https://github.com/nieffka)

---

## 📝 License

This theme is for personal use. Respect the licenses of all included mods.  
CMI is licensed under its own terms—see its [repository](https://github.com/Starry-AXQG/Context-Menu-Icons) for details.

---
