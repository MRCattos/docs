# Troubleshooting
In this troubleshooting section, you can find common problems and fixes for them. 
These issues and fixes come from the official Atlas Discord server. 

## Password not working
After the second restart when completing the the ame wizzard some people need a password to log into their account. <br />
Try **leaving the password empty or type in "atlas"** to see if that works. <br />
If that doesn't work feel free to make a post in the Atlas forum section on the Atlas Discord server.

## Reticulating Splines
After running the Playbook with the AME Wizard some people get stuck at the "Recticulating Splines" screen. <br/>
### First possbible fix:
Check if you have **both the AME Wizard and the playbook on your desktop**. If not, please stop the AME Wizard with Task Manager, move both the Wizard and Playbook to your desktop and try again.
### Second possible fix is to:

1. Open Task Manager.
2. Kill The curl executable,
3. Kill powershell,
4. Kill Windows Command Processor,

Progress should start again

## No image preview ?
1. Enable animations from atlas folder which is located at: `Atlas/3. Configuration/1. General Configuration/Animations`
2. Press the windows key and type "adjust the appearance and performance of windows" and enable "show thumbnails insteaf of icons".
3. Make sure "Always show icons, never thumbnails" is off in the file explorer.

## Hyper-V not working
Some people get "...not found" errors when trying to enable Hyper-V.
### Fixing most not found errors
1. Run "Reset Network to Windows Default" in `Atlas/4. Troubleshooting/Network/`
2. Run `wsl --install` in Powershell as admin
3. Run "Enable Lanman Workstation" in `Atlas/3. Configuration/1. General Configuration/Lanman Workstation (SMB)` and restart your PC.
4. Restart and run "Enable Hyper-V and VBS" in `Atlas/3. Configuration/1. General Configuration/Hyper-V and VBS`
### Service/Driver gcs not found
Make sure something along the lines of "virtualization" is enabled in your bios.
Still have errors ? Make sure to make a post in the atlas-support channel in the discord server.
