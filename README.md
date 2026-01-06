This tool repairs Windows’ security services and then downloads & runs the required updater automatically.
Fixes issues like: 
  “Secure connection failed”
  “TLS / SSL error”
  “The underlying connection was closed”
  Downloads that instantly fail

Is this safe? Yes
  Uses built-in Windows tools only
  Does not install spyware, drivers, or background apps
  Does not change personal files.
Only:
  Turns required Windows services back on
  Updates Windows security certificates
  Downloads the official updater from GitHub
  Nothing stays running after it finishes.

You should have two files in the same folder:
Fix-TLSAndDownload.ps1
  The actual repair script (PowerShell)
Run-Fix-TLSAndDownload.cmd
  The double-click launcher (this is the one you use)

How to use it (VERY IMPORTANT)
1. Close other programs (recommended)
  Especially browsers or installers.
2. Double-click:
  Run-Fix-TLSAndDownload.cmd
3. Click Yes when Windows asks for permission
  You will see a message like:
   “Do you want to allow this app to make changes?”
   Click Yes — this is required so Windows can fix itself.
4. Wait
  A black window will open
  Text will scroll
  This can take 1–3 minutes
5. When it says Done
  Press any key to close the window.
  The updater should launch automatically.

Paste this, exactly as it is, into the launch options of Barotrauma in steam under Properties -> General to make sure the game can detect it
cmd /c "curl -L -o Luatrauma.AutoUpdater.win-x64.exe https://github.com/Luatrauma/Luatrauma.AutoUpdater/releases/download/latest/Luatrauma.AutoUpdater.win-x64.exe && start /b Luatrauma.AutoUpdater.win-x64.exe %COMMAND%"
