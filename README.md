# 🚀 Custom Windows Autounattend (Clean & Debloated)

This repository contains a customized `autounattend.xml` file designed to fully automate the installation of Windows 10/11, strip away bloatware, and optimize the system for maximum performance.

Generated via **[Schneegans](https://schneegans.de/windows/unattend-generator/)** and further customized by **batuhd** for a specific workflow.

## ✨ Key Features

This configuration modifies the standard Windows experience in the following ways:

### 🎨 Visuals & Interface
* **Theme:** **Dark Mode** enabled by default for both System and Apps.
* **Taskbar:** Aligned to the **Left** (Windows 10 style) with Widgets disabled.
* **Context Menu:** Restores the **Classic (Full) Right-Click Menu**, removing the "Show more options" toggle.
* **Wallpaper:** Automatically downloads and applies a custom **7ABR** themed wallpaper from this repository during setup.
* **Explorer:** File extensions and hidden files are visible by default. "This PC" icon added to desktop.

### ⚡ Performance & System
* **Debloat:** Aggressively removes pre-installed bloatware including Candy Crush, Clipchamp, Cortana, Bing News, Skype, Solitaire, Zune, Feedback Hub, and more.
* **Services:** OneDrive, Teams, Office 365, Copilot, and Windows Hello are removed or disabled.
* **Power Settings:** optimized for "High Performance" (Sleep on AC disabled).
* **Mouse:** "Enhance pointer precision" (Mouse Acceleration) is disabled.

### 🛡️ Privacy & Security (Important)
* **Windows Defender:** ⚠️ **Completely Disabled** (via Registry & Service modification).
* **Telemetry:** Tracking and reporting services are disabled.
* **Bypass:** TPM 2.0, Secure Boot, and RAM checks are bypassed (allows installation on older hardware).

## 📦 How to Use

1.  **Get an ISO:** Download a clean Windows 10 or 11 ISO.
2.  **Add the File:**
    * **Using Rufus:** After burning the ISO, copy `autounattend.xml` to the **root** of the USB drive.
    * **Using Ventoy:** Place the XML file in the same directory as your ISO or use the Auto Injection plugin.
3.  **Boot:** Boot from the USB. The installation will proceed **automatically** (only the disk partitioning screen is left manual for safety).

## ⚠️ Disclaimer & Warning

**This configuration disables Windows Defender and Firewall features.**
This is done to free up system resources and prevent interference, but it leaves the system vulnerable to malware and network attacks if not managed correctly.

* **Use at your own risk.**
* It is assumed you have the knowledge to secure your system or understand the risks involved.
* The author is not responsible for any data loss or security breaches resulting from the use of this file.

## 🔧 Customization

If you want to change the computer name (currently set to `Sinop`), keyboard layout, or the list of removed apps, simply open `autounattend.xml` in a text editor (VS Code, Notepad++) and modify the relevant sections.

---
*Maintained by [batuhd](https://github.com/batuhd).*
