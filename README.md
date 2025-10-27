# 🌿 Cozy-Zen

My personal, hand-crafted CSS theme for the [Zen Browser](https://zen-browser.app/), designed for a clean, calm, and highly functional browsing experience.

This theme includes visual refinements, layout tweaks, and integrates the powerful **Context-Menu-Icons (CMI)** mod to bring intuitive icons and smart folding to Zen’s right-click menus.

---

## 📦 Included Mods

### ✨ [Context-Menu-Icons (CMI)](https://github.com/Starry-AXQG/Context-Menu-Icons)
> Adds beautiful FluentUI/ZenUI icons to all context menus — including tabs, bookmarks, extensions, zenFolders, and zenWorkspaces.  
> Includes **JavaScript-powered menu folding** to declutter long menus.

- **Icon Packs**: FluentUI (default) or ZenUI
- **Smart Folding**: Collapse rarely used items into a “Show more options” submenu
- **Hotkey Control**: Toggle folding per item with `CapsLock + Ctrl + Shift + A`
- **Temporary Full Menu**: Hold `Shift` while right-clicking to bypass folding

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
       └── modules/                ← organized mod directory
           └── icons/              ← Context-Menu-Icons (CMI)
               ├── icons.css
               ├── CMI-config.css  ← ✅ customization file (edit this!)
               ├── fluentui/
               └── zenui/
   ```

> 💡 **Important**: The `CMI-config.css` file **must be inside** the `icons/` folder for CMI to load properly.

### 3. Enable Required Preference
In `about:config`, ensure this setting is **enabled**:
```
svg.context-properties.content.enabled = true
```
> ⚠️ CMI will **not run** without this.

### 4. Restart Zen Browser
After copying files and setting preferences, fully restart Zen to apply changes.

---

## ⚙️ Customizing Context-Menu-Icons

Edit `modules/icons/CMI-config.css` to personalize behavior:

```css
:root {
  /* Choose icon pack: 1 = FluentUI (default), 2 = ZenUI */
  --cmi-icon-package: 1;

  /* Fold specific menu items by ID (comma-separated) */
  --cmi-fold-item-ids: "context-openlink, context-openlinkprivate, context-sendlinktodevice";

  /* Customize folded submenu label */
  --cmi-fold-menu-label: "Show more options";
}
```

Alternatively, manage settings via `about:config`:
- `cmi-Switch-Icon-Package` → `1` or `2`
- `cmi-fold-item-IDs` → comma-separated list of menu item IDs
- `cmi-fold_menu_item-enable` → `true`/`false` to toggle folding

> 💡 **Pro Tip**:  
> With the context menu open, hover an item and press **`CapsLock + Ctrl + Shift + A`** to instantly add/remove it from the folded list—no manual ID lookup needed!

> 🕶️ Hold **`Shift`** while right-clicking to temporarily show the full, unfolded menu.

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

---

## 📝 License

This theme is for personal use. Respect the licenses of all included mods.  
CMI is licensed under its own terms—see its [repository](https://github.com/Starry-AXQG/Context-Menu-Icons) for details.

---

> 🌼 Enjoy a cozier, more intuitive Zen experience.
```

--
