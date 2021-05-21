# DDLC-reniOS
DDLC on iOS using RenPy and reniOS support files

Xcode 10.0, macOS 10.14

Ren'Py 6.99.14.3

iOS 14.3, checkra1n 0.12.4, Taurine 1.04


This project uses the Steam installation of DDLC and was put through the Ren'Py Launcher's option to create an iOS distribution. iOS support required the use of iOS support files from RenPy's download page. 

This project was made to be used on jailbroken iOS devices, as the app needed to read and write files. Also, in order to manipulate .chr files or even add mods, you need to view the directories of the application, which is only available for jailbroken handsets.

On the test device, I also changed permissions on the base folder using chmod 777 in order to allow write access. In the end, no tracebacks were encountered.

Tested on iPad 5th generation and iPhone 12 Pro, both on iOS 14.3. Jailbreaks used were Checkra1n 0.12.4 and Taurine 1.04, respectively. The app itself installs as /Applications/DDLCsteamiOS/. There you can find game files in base/.

Theoretically, mods for DDLC can be loaded by placing mod .rpa files into the base/game folder, like you would on Steam games. The mod "Fruits of the Literature Club" was tested this way. Make sure to delete persistent save files in var/mobile/Containers/data/Applications though. Mods that require custom libraries like the Just Yuri mod should not work, however.

Releases should have a deb file compiled from this project, which can be installed using filza file manager or another package manager.

