🔹 1. Download WSA Files

Go to:
https://github.com/MustardChef/WSABuilds

Download:

• WSA_2407.40000.4.0_x64_Release-Nightly-NoGApps-NoAmazon.7z
• WSA_2407.40000.4.0_x64_Release-Nightly-GApps-13.0-NoAmazon.7z

🔹 2. Extract No-GApps Version

• Install 7-Zip or Nanazip
• Right click → Extract the No-GApps file
• Rename folder to: WSA
• Move it to: Documents

Example:
C:\Users\YourName\Documents\WSA

🔹 3. Install Base WSA (If PowerShell Is Not in Right Click)

Method A (Recommended):

• Open the WSA folder
• Click the address bar at the top (where the folder path is)
• Type: powershell
• Press Enter

PowerShell will open in that folder.

Then type:

.\Install.ps1

Press Enter and wait.

Method B (Alternative):

• Click Start
• Type: PowerShell
• Right click → Run as Administrator
• In PowerShell type:

cd C:\Users\YourName\Documents\WSA

(Replace YourName with your Windows username)

Then run:

.\Install.ps1

• Wait until install finishes
• Make sure WSA opens after install

🔹 4. Close WSA

• Close the app
• Or End Task in Task Manager
(Important before next step)

🔹 5. Install Google Play (GApps)

• Extract GApps file
• Copy ALL files
• Paste into WSA folder
• Choose: Replace All

• Run Install.ps1 again (same way as above)

🔹 6. Download ADB (Android Tools)

Download:
https://dl.google.com/android/repository/platform-tools-latest-windows.zip

• Extract ZIP
• Move folder to:

C:\ADB

Inside should be: platform-tools folder

🔹 7. Add ADB to Windows PATH (IMPORTANT)

This lets Windows recognize “adb” command.

1️⃣ Click Start
2️⃣ Type: Environment Variables
3️⃣ Open: Edit the system environment variables
4️⃣ Click: Environment Variables
5️⃣ Under “System Variables” find: Path
6️⃣ Click Edit → New
7️⃣ Paste:

C:\ADB\platform-tools

8️⃣ Click OK on everything
9️⃣ Close CMD and open again

🔹 8. Enable Developer Mode in WSA

• Open Windows Subsystem for Android
• Go to Settings
• Turn ON: Developer Mode

🔹 9. Connect ADB to WSA

• Open CMD
• Type:

adb connect 127.0.0.1:58526

• You will get a popup
• Click Allow / Authorize

• Run command again:

adb connect 127.0.0.1:58526

• It should say “connected”

🔹 10. Enable Window Resize Support

In CMD type:

adb shell settings put global enable_freeform_support 1
adb shell settings put global force_resizable_activities 1

🔹 11. Install Eversolo Control

• Open Play Store inside WSA
• Log in to Google
• Search: Eversolo Control
• Install

✅ DONE.
You can now use Eversolo Control on Windows.