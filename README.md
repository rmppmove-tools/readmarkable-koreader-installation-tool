# READMarkable™ KOReader Installer v26.10.30
# October 2, 2026

## http://readmarkable.org

This desktop application installs **KOReader** and the **Triple-tap AppLoad launcher** on **reMarkable™ Paper Pure**, **reMarkable™ Paper Pro Move**, **reMarkable™ Paper Pro** and **reMarkable™ 2** devices using an intuitive UI over SSH.

**Notice:** *reMarkable™ is a trademark of reMarkable AS. This software and documentation are neither endorsed nor sponsored by, nor affiliated with, reMarkable AS.*

---

## 1. Downloading the Software

## Note: Your reMarkable™ device (RMP Pure, RMPP Move, RMPP) will first need to be switched to Developer Mode before you can use this installation tool. RM 2 devices are already in Developer Mode by default. Please visit the following link on reMarkable™'s website for additional information about Developer Mode https://support.remarkable.com/s/article/Developer-mode

## STARTING WITH VERSION v26.10.29 ACTIVATION CODES ARE **NO LONGER REQUIRED**. THE SOFTWARE WILL AUTOMATICALLY CHECK IF A NEW VERSION IS AVAILABLE FOR DOWNLOAD AND NOTIFY THE USER.

## IMPORTANT: THIS INSTALLER SHOULD NOT BE USED ON A DEVICE WITH OTHER COMMUNITY / 3RD-PARTY PLUGINS/LIBRARIES ALREADY INSTALLED WHICH MAY INTERFERE WITH THE INSTALLATION PROCESS.

## IMPORTANT: BEFORE STARTING INSTALLATION ON YOUR DEVICE - PLEASE BE SURE TO FIRST CHECK IF ANY reMarkable™ SOFTWARE UPDATES ARE AVAILABLE FOR DOWNLOAD AND IF SO PLEASE DOWNLOAD AND LET THE UPDATE GET INSTALLED - PLEASE MAKE SURE THAT THE UPDATE FULLY COMPLETES AND YOUR DEVICE RESTARTS BEFORE ATTEMPTING INSTALLATION

## NOTE: BETA VERSIONS of reMarkable OS have NOT been tested or certified to work with this tool. You are strongly encouraged to use only STABLE VERSIONS of reMarkable OS 

## IMPORTANT - IF YOUR DEVICE HAS JUST GONE THROUGH A **MAJOR** reMarkable OS VERSION UPDATE (EXAMPLE: UPDATING FROM 3.27.x.x TO 3.28.x.x - NOTE THE CHANGE 3.27 TO 3.28) THEN YOU SHOULD NOT USE MAINTENANCE MODE. INSTEAD, USE THE INSTALLER TOOL TO FIRST UNINSTALL KOREADER THEN PERFORM A FULL INSTALLATION OF KOREADER. THIS ONLY APPLIES WHEN A **MAJOR** VERSION UPDATE OCCURS. FOR **MINOR** VERSION UPDATES (EXAMPLE: EXAMPLE 3.28.0.129 TO 3.28.0.132 - NOTE THE MAJOR VERSION NUMBER (3.28) REMAINS THE SAME), THEN YOU SHOULD USE MAINTENANCE MODE TO RE-ENABLE THE APPLOAD AND TRIPLETAP SERVICES ON YOUR DEVICE

## VERY IMPORTANT !!! - DURING BOTH THE FULL INSTALLATION MODE (AT STEP 14) AND THE MAINTENANCE MODE (AT STEP 2) YOU WILL BE PROMPTED TO MANUALLY RESTART YOUR DEVICE IF IT DOES NOT AUTOMATICALLY RESTART ON ITS OWN - PLEASE CAREFULLY WATCH FOR A NOTIFICATION MESSAGE WINDOW AT THESE RESPECTIVE STEPS - IMPORTANT NOTE: BEGINNING WITH reMarkable™ OS VERSION 3.28 ALL DEVICE MODELS WILL NORMALLY AUTOMATICALLY RESTART ON THEIR OWN AT THESE RESPECTIVE STEPS - IF YOUR DEVICE AUTOMATICALLY RESTARTS AT THIS STEP (STEP 14 FULL INSTALLATION / STEP 2 MAINTENANCE MODE) THEN **DO NOT** MANUALLY RESTART THE DEVICE, INSTEAD SIMPLY CLICK OK IN THE NOTIFICATION WINDOW.

Download the correct .zip file version for your specific machine operating system (Windows, macOS) from the READMarkable KOReader Installer landing page:

## http://readmarkable.org

**\*\*ATTENTION macOS USERS: After downloading and unzipping the application file open a Terminal window and execute the following commands:**

**cd /Users/<your_user_name>/Downloads/readmarkable-koreader-installer-macos-arm64**

**chmod +x readmarkable-koreader-installer-macos-arm64**

**Then launch the application in the terminal by executing:**
**./readmarkable-koreader-installer-macos-arm64**

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
   - **reMarkable™ Paper Pure** (AARCH64, 2026)
   - **reMarkable™ Paper Pro Move** (AARCH64, 2025)
   - **reMarkable™ Paper Pro** (AARCH64, 2024)
   - **reMarkable™ 2** (ARMv7, 2020)
  

- **Enter connection info**
   - **Device IP** (default `10.11.99.1` when connected by USB Cable).
   - **SSH password** (shown on the device in *Settings → Help → Copyrights → General information*).

- **Choose Installation Type**
   - **Full Installation**: (UI Sidebar AppLoad + KOReader) **HIGHLY RECOMMENDED**
   - **Maintenance Mode**: Re-enables KOReader, AppLoad and Tripletap on the device after a reMarkable™ software update has occurred
   


## 4. **Installation Options**
   - **Create system backup** (**HIGHLY RECOMMENDED**)
   - **Enable Triple‑tap launcher** (**HIGHLY RECOMMENDED**)

## 5. **KOReader / AppLoad / Tripletap Device Post Software-Update Maintenance Tasks (Maintenance Mode)**
   - **Select this option if you have performed a reMarkable™ device software update**
   - **Re-enables KOReader, AppLoad and Tripletap on the device after a software update has occurred**

## 6. **Install**
   - Click **Install** and watch the live log/progress.
   - When finished, KOReader and/or the launcher will be available on your device. If the launcher is not visible quickly tap the power button 3 times - the device will reboot and the launcher will be visible.

## 7. **Uninstall**
   - Click **Uninstall KOReader** to remove **UI Sidebar AppLoad**, **KOReader**, **Triple-tap launcher** patches, and related files, then reload services.


## 8. Triple‑tap power button AppLoad launcher

Enabling this option installs the **tripletap** service on the device. After install, **triple‑press** the power button within ~3 seconds to start the UI Sidebar Launcher automatically.


## 9. Tips & Troubleshooting

- **“Cannot connect via SSH”** → Confirm the device IP and SSH password, and that the device is reachable over USB or Wi‑Fi.
- **“KOReader file not found / too small”** → Verify your `./nightly/` or `./stable/` file exists and is a valid KOReader zip.
- **Patches not applied** (reMarkable™ Paper Pro Move) → Ensure your `./patch/` or `./patches/` tree exists and contains actual files.


## 10. Contact / Support

- For general help, feel free to open an issue or contact the developer at: **info@rmppmove-tools.org**
