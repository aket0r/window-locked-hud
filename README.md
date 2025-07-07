# WINDOWS HUD LOCKER

A userscript that lets you lock your current browser window with a custom password via a keyboard shortcut.  
Designed to act as a quick-access browser "lock screen" using localStorage and a minimal overlay interface.

## 🔐 Features

- Lock the screen instantly using a keybind: **Ctrl + .**
- Prompts to set a password on first use
- Prevents interaction with the page until unlocked
- Password is securely stored in `localStorage`
- Customizable visuals and logic in script

## 🚀 How It Works

1. Press **Ctrl + .** to activate the lock
2. If no password is set yet — you'll be prompted to create one
3. A translucent HUD overlay will appear, blocking the page
4. Enter your password to unlock and restore interaction

## 🧠 Storage Keys

The script uses `localStorage` under the current domain:

- `LOCKED_WINDOW_HUD_PSWD` — your custom password
- `LOCKED_WINDOW_HUD_PSWD_STATUS` — current lock status (`true` / `false`)

You can view or clear them via browser DevTools:  
→ **Application** tab → **Local Storage** → `https://your-site.com`

## ⚙️ Customization

You can edit the script to change:

- Password prompt text
- Shortcut key (`Ctrl + .`)
- HUD overlay styles (e.g. dark mode, blur)
- Lock/unlock animations or sounds

## 📦 Installation

Install via:
- [GreasyFork](https://greasyfork.org/en/scripts/...) *(if published)*
- Or add the `.user.js` script directly to **Tampermonkey**

## 🧑‍💻 Author

Developed by [aket0r](https://github.com/aket0r)

---

**Note:** This is a visual lock. It’s not designed for strict security or access control — but rather as a quick privacy screen or attention blocker.
