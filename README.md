# 🌿 Cozy-Zen

A personal collection of custom CSS tweaks to make [Zen Browser](https://zen-browser.app/) feel calm, cozy, and perfectly tailored to my workflow.

Zen Browser supports deep UI customization through `userChrome.css`—and this repo is where I experiment, refine, and share my favorite visual enhancements.

## 🎨 Features
- Streamlined interface with reduced visual clutter  
- Soft padding and rounded elements for a “cozy” feel  
- Custom tab styling (vertical or horizontal)  
- Subtle animations and hover effects  
- Optimized for focus and minimal distraction  

> 💡 Inspired by minimalism and mindful computing.

Got it! Based on your instruction, it seems you're actually referring to a **userChrome.css**-style customization for Firefox (not wallpapers), since you mention `custom.css`, `content.css`, and a `modules` folder inside a `chrome` directory.

However, your GitHub repo is titled **Minimalistic-desktop-wallpapers**, and currently contains no code or files (based on the knowledge base). If you're updating the README for a **Firefox theme/mod** instead, here’s a revised **Installation section** you can use in your `README.md`:

---

### 🛠️ Installation

1. **Enable Firefox userChrome support** (if not already enabled):
   - Go to `about:config`
   - Set `toolkit.legacyUserProfileCustomizations.stylesheets` to `true`

2. **Locate your Firefox profile folder**:
   - Go to `about:support`
   - Under **Application Basics**, find **Profile Folder** → click **Open Folder**

3. **Create or open the `chrome` folder** inside your profile folder.

4. **Copy the following into the `chrome` folder**:
   - `userChrome.css`
   - `userContent.css`
   - The entire `modules` folder

   Your structure should look like this:
   ```
   your-firefox-profile/
   └── chrome/
       ├── userChrome.css
       ├── userContent.css
       └── modules/
           ├── Sidebar.css
           └── ... (other module files)
   ```

5. **Restart Zen** to apply the changes.

## Integrated Mods

This theme includes the following community mods for enhanced UI:

### Context Menu Icons (CMI)
- **Source**: [Starry-AXQG/Context-Menu-Icons](https://github.com/Starry-AXQG/Context-Menu-Icons)
- **Version**: v2.1+
- **Features**:
  - Adds intuitive icons to Zen browser’s context menus (including zenFolder and zenWorkspace).
  - Supports **FluentUI** and **ZenUI** icon packs (default: FluentUI).
  - Extensions, bookmarks, and tab context menus are visually harmonized.

#### How It’s Integrated
- The `icons/` folder (from CMI) is placed inside the `chrome/modukes` directory.
- Loaded via:  
  ```css
 @import "modules/CMI/CMI-config.css";
 @import "modules/CMI/icons.css"; ```

---

Let me know if you'd like this integrated into a full README, or if the repo actually *does* include these files (they’re just not visible in the current GitHub view).

## 📜 License
This CSS customization is free to use, modify, and share.  
Licensed under **MIT**—see [LICENSE](LICENSE) for details.
