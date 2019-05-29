This readme file explains how to use the compiled Windows executable called themerandom.exe

NOTE:	Windows Defender may delete the 'themerandom.exe' file. You will need to disable your defence to keep this file. 

Using this option means every time you start your Windows Emulation Station, it will select a random theme from any of the themes you have installed.
Keeping your Emulation Station fresh and exciting.

1. To follow ar the details and instructions found from files in the archive called themerandom_windows_es.zip
2. Unzip the archive anywhere on your computer
3. The archive should contain this readme file, a compiled AutoHotkey file called themerandom.exe, and a themerandom.ini file
4. You need to modify the 'ThemeRandom.ini' file (NOT the .exe file) to include two paths which matches to your Emulation Station for Windows installation

	i) Edit ThemeRandom.ini with any convenient text editor
	
	ii) Find the first line to edit: ThemeHomeDir=
	
	iii) Append the full path to your Emulation Station themes directory
	
	iv) An example of the finished line may be: ThemeHomeDir=D:\Games\Portable_Game_Station_1.5\.emulationstation\themes
	
	v) Find the second line to edit: ESConfig=
	
	vi) Append the full path to your Emulation Station configuration file
	
	vii) An example of the finished line may be: D:\Games\Portable_Game_Station_1.5\.emulationstation\es_settings.cfg
	
	viii) Save the ini file
	
5. Find the DOS batch file (.bat) located in your Emulation Station folder that starts your Emulation Station program
6. There are usually 2 of these. One for full screen and one for windowed e.g. 'Launch Portable (Fullscreen).bat'
7. Copy and paste the one you use (or both if you use either) in the same directory
8. Give the file/s different name e.g. 'Launch Portable (Fullscreen) RANDOM.bat'
9. Edit the batch file/s in any convenient text editor

	i) add 'themerandom.exe' as a new line above the emulationstation.exe line and below the set HOME=%~dp0 line
	
	ii) An example of the finished batch file would be:
	
		set HOME=%~dp0
		themerandom.exe
		emulationstation.exe
		
	iii) Save the edited batch file
	
10. Select and COPY the 2 files from the archive: 'ThemeRandom.ini' & 'themerandom.exe'
11. PASTE these 2 files in the same directory as the batch file (your Emulation Station folder)
12. Launch Emulation Station with the new edited batch file (e.g. Launch Portable (Fullscreen) RANDOM.bat)
13. Emulation Station should boot with a random theme you have installed each time you boot it up
