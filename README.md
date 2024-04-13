# WindowsTerminalQuakeAutostart
My way to get Windows Terminal to start in Quake mode in the background on Windows startup/login.

##
My default terminal profile is Powershell (Admin), which causes some problems for autorun.
I'm using .bat file which opens Terminal minimalized "/min" in quake mode "-w _quake".

## Instalation
Create .bat file as example WTQ_bat.bat wherever you like.

### Create Windows Task

1. Open Windows Task Scheduler (C:\ProgramData\Microsoft\Windows\Start Menu\Programs\Administrative Tools)
2. Create Task
   -    In the General tab, enter task name and if you want to run Terminal in Administrator mode, tick the checkbox "Run with highest privileges".
   -    In the Trigger tab create new and select "Begin the task:" as "At log on".
   -    In the Action tab create new Action Start a program and Program/sreipt select .bat file.
   -    In Conditions tab unselect everything.
   -    In Settings tab default options should be fine.
