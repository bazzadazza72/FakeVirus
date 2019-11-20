This is the readme file for FakeVirus. It is recommended that you read it entirely so you know what goes on.

It is an exact (with some slight differences) copy from the readme file that is included in the compiled archive.

---------- How to install ----------

To install FakeVirus, run the installer (fv_installer.exe) via the "installer" folder inside the main folder where this readme file is.
You may need to provide authentication for administrator access (except Windows XP).

Note: Windows XP or later is required. A version of FakeVirus for Windows 95/98 can be found here:
*insert link here*

If you want to install FakeVirus onto a computer without administrator access, run the fv_stealth.exe file
(in the "installer" folder) to install FakeVirus. No GUI will appear and internet access isn't required.

If you want to install FakeVirus onto a computer with administrator access but no internet access,
hold the Shift key when you run the installer.

Both versions install by default. To override this, hold 1 (for voice) or 2 (for textbox) when the installer starts.
A text box will appear showing which version you have selected before it starts copying.

---------- Version differences ----------

Voice only - No text boxes appear and only text to speech is played. A shortcut disguising
as Windows Explorer will be created.

Textbox only - No text to speech is played and only a sequence of textboxes are displayed. A shortcut disguising
as Windows Explorer will be created.

Both - FakeVirus installs itself into the Task Scheduler library (run at startup) and uses a combination of text to speech phrases and textboxes.
Depending on the system's time, various payloads will occur, such as screen color inverting, background picture changes and much more.


---------- Error codes ----------

An error dialog will appear when the FakeVirus installer has encountered a problem.

Error dialogs (error code E00 and E01) only appear when FakeVirus is initalizing.

Error codes (and information about them) are listed below:

E01 - The installation process failed because the copied files couldn't be verified. Make sure the listed file(s)
have a correct signature (you can find out what a signature is and compare them here: __)

E00 - The files required for FakeVirus couldn't be verified. Make sure the listed file(s) have a correct
signature (you can find out what a signature is and compare them here: __)

E10 - The computer's internet connection is unreliable. Check the computer's connection to the internet. Try running
the fv_stealth.exe installer file, check How to install for more info.

E12 - The available space on the computer's hard disk is low. Make sure there is at least __ MB to install FakeVirus.

E15 - The installation process failed because the required files couldn't be copied. Make sure the installer is being run
in an elevated mode (as an administrator) and make sure the installation directory has read and write permissions set correctly.

E16 - An incorrect value has been set in the configuration file. Make sure the configuration value is correct before starting
the FakeVirus installer. Check Configuration help for more info. This error only occurs at startup.

E17 - The configuration file for the FakeVirus installer could not be read. Make sure this file is in the same directory
as the installer and make sure the permissions are set correctly for reading the file.


---------- Configuration help ----------

The configuration file (fv_installer.ini) must be in the same directory as the installer (the installer won't function at all if it isn't there)

[INTERNAL] - Section for FakeVirus installer configuration ([AHK2EXE] and [VERSION] are configuration sections for the compiled EXE, edit these at your own risk)

CustomInstallDir - Specifies a different installation directory. (default is C:\FV)
(0 = use default directory)
This value can be ommitted (left without a value).

CustomTempDir - Specifies a different temporary directory for downloaded files during installation. (defualt is C:\FV\Temp)
(0 = use default directory)
This value can be ommitted (left without a value).
