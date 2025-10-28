# READMarkable KOReader Installer v0.1.11-rc1 
# &nbsp; &nbsp; &nbsp; LIMITED RELEASE CANDIDATE TESTING PHASE

**• NOTICE: THIS IS RELEASE CANDIDATE TESTING SOFTWARE UNDER ACTIVE DEVELOPMENT - SOFTWARE BUGS MAY BE PRESENT
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;USE FOR TESTING PURPOSES ONLY**

This desktop application installs **KOReader** and the **Triple-tap AppLoad launcher** on **reMarkable™ Paper Pro Move**, **reMarkable™ Paper Pro**, and **reMarkable™ 2** devices using an intuitive UI over SSH.

**Notice:** *reMarkable™ is a trademark of reMarkable AS. This software and documentation are neither endorsed nor sponsored by, nor affiliated with, reMarkable AS.*

---

## 1. Downloading the Software

## Note: Your reMarkable™ device (RMPP Move, RMPP) will first need to be switched to Developer Mode before you can use this installation tool. Please visit the following link on reMarkable™'s website for additional information about Developer Mode https://support.remarkable.com/s/article/Developer-mode

## IMPORTANT - STARTING WITH THIS RELEASE - DURING INSTALLATION YOU MAY BE PROMPTED TO MANUALLY RESTART YOUR DEVICE IF IT DOES NOT AUTOMATICALLY RESTART ON ITS OWN - PLEASE WATCH FOR A NOTIFICATION MESSAGE WINDOW

Download the correct .zip file version for your specific machine operating system (Windows, MacOS) from the following download links:

Windows:  https://rmppmovetools.blob.core.windows.net/rmppmove-tools/readmarkable-koreader-installer-windows-amd64.zip

MacOS:    https://rmppmovetools.blob.core.windows.net/rmppmove-tools/readmarkable-koreader-installer-macos-arm64.zip

**\*\*Attention MacOS Users: After downloading and unzipping the application file open a Terminal window and execute the following commands:**

**cd /Users/<your_user_name>/Downloads/readmarkable-koreader-installer-macos-arm64**

**chmod +x readmarkable-koreader-installer-macos-arm64.app**

**chmod +x readmarkable-koreader-installer-macos-arm64**

**After doing that you should be able to double-click on either of those two files and the application should launch without issue.**

---

## 2. What this software application does

- Full KOReader install using **local zip files** (no KOReader downloads during install).
- Installs/updates the UI Sidebar AppLoad.
- Installs **Triple‑tap power button** shortcut to launch the UI Sidebar AppLoad.
- Automatic **system backup** before changes (optional).
- **One‑click Uninstall** to restore stock state (removes UI Sidebar AppLoad/KOReader).
- **Post‑install patches** for **All Devices** from `./patch/` or `./patches/` (if present).
-  **system backup** before changes (optional).
- Performs **Device Post Software-Update Maintenance Tasks** to re-enable KOReader, AppLoad and Tripletap on the device after a software update has occurred.


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
   - **Full Installation**: (UI Sidebar AppLoad + KOReader) **HIGHLY RECOMMENDED**
   - **Launcher Only Installation**: UI Sidebar Launcher Only (UI Sidebar AppLoad)


## 4. **Installation Options**
   - **Create system backup** (**HIGHLY RECOMMENDED**)
   - **Enable Triple‑tap launcher** (**HIGHLY RECOMMENDED**)

## 5. **KOReader / AppLoad / Tripletap Device Post Software-Update Maintenance Tasks**
   - **Select this option if you have performed a device software update**
   - **Re-enables KOReader, AppLoad and Tripletap on the device after a software update has occurred**

## 6. **Install**
   - Click **Install** and watch the live log/progress.
   - When finished, KOReader and/or the launcher will be available on your device.

## 7. **Uninstall**
   - Click **Uninstall KOReader** to remove **UI Sidebar AppLoad**, **KOReader**, **Triple-tap launcher** patches, and related files, then reload services.


## 8.  Activation

- For Beta Software Testing Purposes This Application Uses An Activation Code Restricting Use To Your **Machine ID**.
- Default **Beta software testing duration** is **14 days**.


## 9. Triple‑tap power button AppLoad launcher

Enabling this option installs the **tripletap** service on the device. After install, **triple‑press** the power button within ~3 seconds to start the UI Sidebar Launcher automatically.


## 10. Tips & Troubleshooting

- **“Cannot connect via SSH”** → Confirm the device IP and SSH password, and that the device is reachable over USB or Wi‑Fi.
- **“KOReader file not found / too small”** → Verify your `./nightly/` or `./stable/` file exists and is a valid KOReader zip.
- **Patches not applied** (reMarkable™ Paper Pro Move) → Ensure your `./patch/` or `./patches/` tree exists and contains actual files.


## 11. Contact / Support

- For activation assistance, use the instructions shown in the application's activation dialog.
- For general help, feel free to open an issue or contact the developer at: **info@rmppmove-tools.org**
