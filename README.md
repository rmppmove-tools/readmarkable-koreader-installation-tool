# READMarkable KOReader Installer v0.1.6-dev

This desktop application installs **KOReader** and the **XOVI Triple-tap AppLoad launcher** on **reMarkable™ Paper Pro Move**, **reMarkable™ Paper Pro**, and **reMarkable™ 2** devices using an intuitive UI over SSH.

**Notice:** *reMarkable™ is a trademark of reMarkable AS. This software and documentation are neither endorsed nor sponsored by, nor affiliated with, reMarkable AS.*

---

## 1. Downloading the Software

Download the correct .zip file version for your specific machine operating system (Windows, MacOS) from the following download links:

Windows:  https://drive.google.com/file/d/1D71u0fmIge-DyV6iMgb8DsbwQNSbNBRK/view?usp=sharing

MacOS:    https://drive.google.com/file/d/1NVaDkgTbtrNXnrEEeWId5MDNU7hOIkSe/view?usp=sharing

---

## 2. What this software application does

- Full KOReader install using **local zip files** (no KOReader downloads during install).
- Installs/updates the XOVI launcher and AppLoad.
- Installs **Triple‑tap power button** shortcut to launch XOVI AppLoad in the UI.
- Automatic **system backup** before changes (optional).
- **One‑click Uninstall** to restore stock state (removes XOVI/AppLoad/KOReader).
- Optional **post‑install patches** for **Remarkable Paper Pro Move** from `./patch/` or `./patches/` (if present).


## 3. Using the Software

- **Start the application**

- **Pick your device model**
   - **reMarkable™ Paper Pro Move** (ARM64, 2025)
   - **reMarkable™ Paper Pro** (ARM64, 2024)
   - **reMarkable™ 2** (ARM32, 2020)

- **Enter connection info**
   - **Device IP** (default `10.11.99.1` when connected by USB Cable).
   - **SSH password** (shown on the device in *Settings → Help → Copyrights → General information*).

- **Choose Installation Type**
   - **Full**: XOVI + AppLoad + KOReader (**HIGHLY RECOMMENDED)
   - **Launcher only**: XOVI + AppLoad (no KOReader changes)
   - **Stage 1 only**: Base setup (through hashtable)
   - **Stage 2 only**: KOReader installation

## 4. **Options**
   - **Create system backup** (**HIGHLY RECOMMENDED)
   - **Enable Triple‑tap launcher** (**HIGHLY RECOMMENDED)

## 5. **Install**
   - Click **Install** and watch the live log/progress.
   - When finished, KOReader and/or the launcher will be available on your device.

## 6. **Uninstall**
   - Click **Uninstall** to remove **XOVI**, **AppLoad**, **KOReader**, patches, and related files, then reload services.


## 7.  Activation

- The app uses activation tied to your **Machine ID**.
- Default **Beta software testing duration** is **14 days**.


## 8. Triple‑tap power button AppLoad launcher

Enabling this option installs the **xovi‑tripletap** service on the device. After install, **triple‑press** the power button within ~3 seconds to launch XOVI AppLoad automatically.


## 9. Tips & Troubleshooting

- **“Cannot connect via SSH”** → Confirm the device IP and SSH password, and that the device is reachable over USB or Wi‑Fi.
- **“KOReader file not found / too small”** → Verify your `./nightly/` or `./stable/` file exists and is a valid KOReader zip.
- **Patches not applied** (reMarkable™ Paper Pro Move) → Ensure your `./patch/` or `./patches/` tree exists and contains actual files.
- **Triple‑tap not working** → Check the `xovi-tripletap` service status on the device (`systemctl status xovi-tripletap`).
- **Uninstall didn’t remove everything** → Run **Uninstall** again; the app stops services, removes XOVI/AppLoad/KOReader/shims/tripletap, and reloads systemd.


## 10. Support

- For activation assistance, use the instructions shown in the application's activation dialog.
- For general help, feel free to open an issue or contact the developer at: info@rmppmove-tools.org
