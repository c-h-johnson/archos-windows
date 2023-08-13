             Synaptics Touchpad Driver for Windows 2000 / WinXP
                        Installation Notes
                         Version 7.12.7
                              
1. Installing the Synaptics TouchPad Driver
-------------------------------------------

This driver requires Windows 2000 / WinXP.

NOTE REGARDING SAVING OF SETTINGS:
----------------------------------
Windows 2000 / WinXP does not save any of the user settings for users
belonging to the "Guests" user group. This includes special TouchPad
settings as well as all other user settings. If you want your 
settings to be saved, make sure your user account does not belong to 
the "Guests" group using the User Manager program (you must be 
Administrator to change user settings).

Installation procedure
-------------------------------------------------------
First, if you have a new TouchPad, plug it in and reboot Windows 2000 /
WinXP.  Windows 2000 / WinXP will then detect your new TouchPad and 
install a standard mouse driver to handle it. You cannot install the
Synaptics TouchPad driver until this process is complete and your 
TouchPad is functioning as a normal pointing device.

Log on to your system as "Administrator", or as another user with 
administrator privileges. 

Run "Setup.exe". This program will automatically install the Synaptics
TouchPad driver to handle all PS/2 and Serial pointing devices
attached to your computer.

You will need to restart Windows after the installation is complete.
If the driver has been installed correctly, after you have restarted 
Windows you should see the TouchPad Icon in your task bar next to the 
clock.  Also, a dialog box entitled "Information about your TouchPad" 
will pop up. You can prevent this dialog box from coming up in the 
future by checking the "Stop showing me this message" checkbox. 

For help using your TouchPad, choose "Tell me more..." from the
"Information about your TouchPad" dialog box, or double-click on the
TouchPad Icon in your task bar, and click on the "Help" button.

If you wish to change one or more of your pointing devices to using 
a standard Microsoft or other third party driver, you should bring
up the Mouse control panel, and select the "Hardware" tab. From there,
select the pointing device you want to change and click "Properties".
Select the "Driver" tab and Click "Update Driver...". Follow the 
instructions to install a new driver.

A few notes on using Setup.exe:
--------------------------------------------

- When using long path and filename expressions with switches, enclose the 
expressions in double quotation marks. The enclosing double quotes tell the 
operating system that spaces within the quotation marks are not to be treated 
as command line delimiters. 

- Do not leave a space between command line switches and options.

- When InstallShield Silent runs, a log file is created in the same folder as 
the response file. The log file has the default name Setup.log if the -f2 switch 
is not provided.

If you are running "Setup.exe" from a CD, you must specify the name and 
a different path for the log file. The default path provided by InstallShield 
is the directory containing "Setup.iss".  If run from a CD, this would result 
in an error, because CDs are read-only. For example, execute the following to run a 
silent install and generate the log file "SynSetup.log" in the C:\Mydir folder:

setup.exe -s -f2"c:\Mydir\SynSetup.log"

To verify that a silent setup succeeded, look at the ResultCode value in the 
[ResponseResult] section of the log file. ResultCode = 0 means the 
installation was successful. 

- If the -f1 switch is not used when running InstallShield Silent, Setup looks for the 
response file Setup.iss in the same folder as Setup.exe. A log file is created in the 
same folder.

- Setup.exe command line switches/options are not case sensitive.



