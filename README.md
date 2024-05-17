# Lavis - RAT over Discord

Lavis is a Python based malware that uses Discord to communicate

# Features

### UAC Bypass - currently only one method but soon will be three

### Sanctions - BSOD, blocking input, logoff and shutdown

### AutoBlacklist - Fully persistent blacklisting

### File Transfer - Upload/Download whenever you want

### File Navigation - Fully operational

### File running - Run files in 2 ways

### Information Gathering - Screenshots, discord token, clipboard and much more!

### Process Management - List and kill processes

### Shell - Sse powershell commands

### Startup - Add to startup with or without admin privs (Thanks to the UAC bypass feature)

### Voice Channel - listen to the target's microphone in real time

### UAC Stuff - Mask the RAT as a windows process (if the target tries to end it he will bsod)

## List of commands
upload [link] - Downloads a file to the victim's pc via link. Only direct link to exe works, tested with github raw download
download [filename] - Uploads the selected file to discord
dw_gofile [filename] - uploads the selected file to gofile and sends the downlaod link
cwd - Returns the current working directory (cwd)
ls - Lists the files in the cwd
cd [folder] - Changes the cwd to a new one
run [filename] - Opens a file using subprocess.popen
run2 [filename] - Opens a file using os.startfile
screenshot - Sends a screnshot of the victim's PC (All monitors)
screenrec - Records a video of the victim's screen (All monitors)
grabber - Currently working on final touches
idle - Returns if the victim is idle and if so, for how much time
clipboard - Sens the victim's current clipboard
edit_clipboard [message] - Edits the victim clipboard
powershell [command] - Calls powershell and executes the given command
uac_startup - Next time the RAT starts it will execute akagi quitely and elevate to have admin privs on startup
uac_crit_startup - Next time the RAT starts it will execute akagi quitely and elevate to have admin privs and mask itself as a Windows process i.e the victim will BSOD if he tries to end it
uac_no_startup - Clears any uac startup configs
startup [name] - Adds the RAT to startup
listenmic - Joins a channel and outputs the victim's Microphone
leave - Leaves the channel
autoblacklist - Shows which processes are in the autoblacklist task
autoblacklist_add [process name] - Adds a process to be persisntently killed
autoblacklist_clear - Clears all given processes
blacklist [process name] - (Supports only on process at a time) - Blacklists the given process name for the current session only i.e if the bot restarts (so will the RAT) the blacklist task will be stopped
blacklist_stop - Stops the blacklist task
show_ping - Shows the ping
exit - Exits the bot
bsod - BlueScreens the victim's PC
block_input - Suppresses mouse and keyboard i.e victim dont have mouse and kb control
unblock_input - Gives back control to the victim
logoff - Calls shutdown /l /f
shutdown - Calls shutdown /p
admin - Tells if the victim is running the RAT as admin
akagi - UAC Bypass | Creates a second instance of the RAT with admin privs and closes the first one
crit - Masks the RAT's process as Widnows process i.e if the user tries to end it he will BSOD
uncrit - Makes the RAT's process normal

## TO DO
Finish and optimize the grabber func
Import more UAC Bypasses (Currently one is used, soon there will three more for sure)
New functions (Feel free to give me ideas)
Import ngrok
Optimise the file size 

## Changelog
**Ver 0.5 - Autoblacklist feature**
**Ver 1.0 - UAC Bypass feature**
