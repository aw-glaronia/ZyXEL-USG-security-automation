# ZyXEL-USG-security-automation
ZyXEL USG Security Automation
This repo includes a collection of security-scripts that could be run by ZyXEL USG Shell Scheduler, to prevent security issues.

## Installation by ZyXEL GUI
`install_task_GUI.zysh` could be used to install Tasks by GUI. Simply Edit the Script as desired, upload it to the ZyXEL USG (Maintenance -> File Manager -> Shell Script) select it and click "Apply"

## Manual Installtion by Console-Access
After Uploading the Script to the ZyXEL USG. Get access to the console. (Doesn't matter if SSH, Telnet, Serial or Smoke-Signs 🤣)
Execute following Commands:

`configure terminal`

`schedule-run 1 firewall_on.zysh daily 02:00`

If you like to verify the scheduled task you could use following command: `show schedule-run`

To Remove the scheduled task simply use: `no schedule-run 1`

### Source
https://www.zyxel.ch/de/support/download/60016
