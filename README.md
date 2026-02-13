==================================================

STEP 1: DOWNLOAD WSA BUILDS

Go to:
https://github.com/MustardChef/WSABuilds

Download:

- WSA_2407.40000.4.0_x64_Release-Nightly-NoGApps-NoAmazon.7z
- WSA_2407.40000.4.0_x64_Release-Nightly-GApps-13.0-NoAmazon.7z

==================================================

STEP 2: EXTRACT NO-GAPPS BUILD

1. Right click No-GApps file and extract
2. Rename folder to: WSA
3. Move it to:

C:\Users\YourName\Documents\WSA

==================================================

STEP 3: INSTALL BASE WSA

1. Open WSA folder
2. Click address bar
3. Type: powershell
4. Press Enter

Run:

.\Install.ps1

Wait until install finishes.

==================================================

STEP 4: CLOSE WSA

Close Windows Subsystem for Android
Or end it in Task Manager

==================================================

STEP 5: INSTALL GOOGLE PLAY (GAPPS)

1. Extract GApps archive
2. Copy all files
3. Paste into WSA folder
4. Replace All
5. Run Install.ps1 again

==================================================

STEP 6: INSTALL ADB

Download:
https://dl.google.com/android/repository/platform-tools-latest-windows.zip

Extract to:

C:\ADB

==================================================

STEP 7: ADD ADB TO PATH

1. Open Start Menu
2. Search: Environment Variables
3. Open system environment variables
4. Click Environment Variables
5. Under System Variables select Path
6. Click Edit > New
7. Add:

C:\ADB\platform-tools

8. Click OK and restart CMD

==================================================

STEP 8: ENABLE DEVELOPER MODE

Open Windows Subsystem for Android
Open Settings
Enable Developer Mode

==================================================

STEP 9: CONNECT ADB

Open CMD

Type:

adb connect 127.0.0.1:58526

Authorize popup

Run again:

adb connect 127.0.0.1:58526

You should see "connected"

==================================================

STEP 10: ENABLE WINDOW RESIZE

Type in CMD:

adb shell settings put global enable_freeform_support 1
adb shell settings put global force_resizable_activities 1

==================================================

STEP 11: INSTALL EVERSOLO CONTROL

1. Open Play Store inside WSA
2. Log in to Google
3. Search: Eversolo Control
4. Install

==================================================

FINISHED

Eversolo Control now runs on Windows 11.

==================================================
