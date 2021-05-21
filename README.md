# DDLC-reniOS
DDLC on iOS using RenPy and reniOS support files

Xcode 10.0, macOS 10.14

Ren'Py 6.99.14.3

iOS 14.3, checkra1n 0.12.4


This project uses the Steam installation of DDLC and was put through the Ren'Py Launcher's option to create an iOS distribution. iOS support required the use of iOS support files from RenPy's download page. 

This project was made to be used on jailbroken iOS devices, as the app needed to read and write files. Also, in order to manipulate .chr files or even add mods, you need to view the directories of the application, which is only available for jailbroken handsets.

When testing, tracebacks were encountered where additional files could not be created. Upon finishing a runthrough of DDLC, I also noticed that the .chr files of sayori, yuri, and natsuki were not deleted. I tried to solve this by giving the app root permissions, obtained using instructions from this link: https://stackoverflow.com/questions/7841344/gaining-root-permissions-on-ios-for-nsfilemanager-jailbreak/8796556#8796556.

On the test device, I also changed permissions on the base folder using chmod 777 in order to allow write access. In the end, no tracebacks were encountered.

Tested on iPad6,11 using Checkra1n 0.12.4 beta. The app itself installs as /Applications/DDLCsteamiOS/. There you can find game files in base/.

Theoretically, mods for DDLC can be loaded by placing mod .rpa files into the base/game folder, like you would on Steam games. The mod "Fruits of the Literature Club" was tested this way. Make sure to delete persistent save files in var/mobile/Containers/data/Applications though. Mods that require custom libraries like the Just Yuri mod should not work, however.

Releases should have a deb file compiled from this project, which can be installed using filza file manager or another package manager.

