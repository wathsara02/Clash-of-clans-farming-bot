# 🛡️ Clash of Clans Farming Bot

A smart farming automation bot for Clash of Clans that:

- Automatically starts searching or attacking.
- Uses OCR for loot detection.
- If the detected loot exceeds a threshold:
  - Deploys Electro Dragons, Balloons, Rage Spells, Heroes, and Siege Machines.
- After the attack, detects the collected loot and returns home.
- Repeats this process until the user stops.
- Protects usage via Firebase-bound license key.
- Comes with a beautiful Tkinter GUI.

---

## 🚀 Features

- ✅ **License Key Binding** (PC-based binding with Firebase)
- 🧠 **Smart Loot Detection** using OCR (Tesseract)
- 🛡️ **Auto-deploy Troops, Spells, Heroes, Siege**
- 💬 **Firebase-hosted News Panel**
- 📊 **Live Stats Dashboard**: Loot totals & attack count
- ✨ **Customizable Parameters**: Gold, Elixir thresholds, troop counts
- 🎮 **Full GUI**: Built with themed `tkinter` and `ttk` components
- 🔐 **Encrypted API URLs** for security

---

## 🧠 Technologies Used

| **Tech**             | **Purpose**                                 |
|----------------------|---------------------------------------------|
| Python 3.x           | Core Programming Language                   |
| Tkinter / ttk        | GUI Framework                               |
| OpenCV               | Image Preprocessing                         |
| pytesseract          | OCR for reading loot                        |
| PyAutoGUI            | Mouse control for game interaction          |
| keyboard             | Keyboard automation                         |
| Firebase Realtime DB | License validation and news system          |
| Requests             | HTTP requests to Firebase                   |
| PIL (Pillow)         | Image handling                              |
| threading            | For async bot operations                    |

---

## 🔐 License Activation

- On first run, you’ll be prompted for a **license key**.
- License is validated with Firebase and bound to your device (`hostname_node`).
- If valid and not already used on another device, it activates.
- **Universal key**: `PC-FORGE` works on any device.

---

## 🛠️ How It Works (Workflow)

### 🔑 License Validation
- Checks the entered key with Firebase, decrypts the URL via XOR logic.

### 🖼️ GUI Initialization
- Loads themed Tkinter interface with:
  - Live logs
  - Parameter sliders
  - News ticker
  - Custom troop settings

### ⚔️ Bot Execution
- Scans loot using screenshot → OpenCV → OCR.
- Compares to user-set threshold.
- If loot is sufficient:
  - Starts attack.
  - Deploys troops (Electro Dragons, Balloons).
  - Drops Rage Spells, Heroes, Siege.
  - Waits and collects post-battle loot stats.

### 🔁 Auto-updates
- Firebase-powered news bar.
- Stats updated live.

---

> ⚠️ **Disclaimer**: This bot automates gameplay and may violate Clash of Clans' terms of service. Use at your own risk. Intended for educational and personal use only.