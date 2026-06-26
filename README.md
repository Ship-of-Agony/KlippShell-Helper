# KlippShell Helper - Unlock advanced functions via ADB commands

A lightweight, multi-language Windows utility designed to unlock advanced system features for the [KlippShell4Creality](https://github.com/Ship-of-Agony/KlippShell4creality) application on Android TV and Fire TV devices.

This helper utility belongs to the core **[KlippShell4Creality Project](https://github.com/Ship-of-Agony/KlippShell4creality)** developed by **Ship of Agony LABs**.

---

## 🚀 Features

The tool automates the setup of advanced permissions via ADB (Android Debug Bridge), removing the need to manually enter complex console commands for the main application:

* **[1] Enable Native PiP (Picture-in-Picture):** Allows the app to run as a compact, floating video window on top of other applications (e.g., while streaming or browsing).
* **[2] Enable TV Overlay (Floating Window):** Unlocks the system overlay permission (`SYSTEM_ALERT_WINDOW`), enabling KlippShell to flexibly display dashboard status information.
* **[3] Allow Background Activity:** Adds the app to the Android system's "Doze Whitelist". This prevents the operating system from unexpectedly closing the background service while in standby.
* **[4] ENABLE ALL 3 FEATURES:** Automatically executes all the above steps sequentially (Recommended).
* **[5] REVOKE ALL PERMISSIONS (Reset / Undo):** Reverts all modified permissions on your TV back to their original factory defaults.

---

## 📦 Downloads & Installation

In the **Releases** section, you will find two ways to utilize this tool:

### Option A: All-in-One EXE (Recommended)
* Download `KlippShell_Helper.exe`.
* **Advantage:** No additional files required. The ADB infrastructure is fully embedded within the executable file and runs automatically in the background.

### Option B: Manual Batch Version (Optional)
If you prefer to inspect the source code or run the script directly, download the ZIP archive. It contains:
* `KlippShell_Helper.bat` (The original batch script)
* `adb.exe` + the required `.dll` files
* **Note:** The `.bat` file must be located in the exact same folder as the `adb.exe` to function correctly.

---

## 🛠️ TV Prerequisites

For the tool to establish a connection to your television, **ADB Debugging** must be enabled:

1. Open the **Settings** on your Android TV / Fire TV.
2. Navigate to **System** (or *My Fire TV*) -> **About**.
3. Click **Build** (or *OS Version*) 7 times consecutively until the message *"You are now a developer"* appears.
4. Go back to settings, open the newly unlocked **Developer Options**, and enable **ADB Debugging** (and *Allow apps from unknown sources* if applicable).
5. Note down the **IP address** of your TV (found under *Settings -> Network*).

---

## 💻 How to Use

1. Launch `KlippShell_Helper.exe` (or the `.bat`). The utility automatically detects your Windows system language and adjusts the interface accordingly.
2. Select your desired option from the menu (Type the corresponding number and hit Enter).
3. Enter your television's IP address.
4. **Important:** Look at your TV screen now! A security prompt will appear. Check the box for **"Always allow from this computer"** and confirm with **OK**.
5. The tool will execute the commands and provide direct feedback (`[OK] - Successfully executed`).

---

## 🌐 Supported Languages

The tool is fully localized and automatically adapts to your PC's system language. The following languages are natively supported:
* 🇩 German (Deutsch)
* 🇺🇸 English (Default Fallback)
* 🇨🇿 Czech (Čeština)
* 🇫🇷 French (Français)
* 🇪🇸 Spanish (Español)
* 🇵🇱 Polish (Polski)
* 🇷🇺 Russian (Русский)

---

## 🔒 Security & Safety

This utility does not modify any core system files and does not require root privileges on your television. It exclusively utilizes official Android developer commands (`appops` / `dumpsys`), which can be completely undone at any time using the built-in reset feature (Option 5).
