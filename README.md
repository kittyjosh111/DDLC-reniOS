# DDLC-reniOS
DDLC on iOS using RenPy and reniOS support files

Xcode 10.0, macOS 10.14

Ren'Py 6.99.14.3

iOS 14.3, checkra1n 0.12.4, Taurine 1.04


This project uses the Steam installation of DDLC and was put through the Ren'Py Launcher's option to create an iOS distribution. iOS support required the use of iOS support files from RenPy's download page. Is to be used in conjunction with my DDLC-reniOS Mod Manager (DDLCRMM), which simplifies fixing problems with the app and injecting mods. It can be found on Routinehub: https://routinehub.co/shortcut/9204/

I heavily recommend using the shortcut, as there is an option to "initialize DDLC", which repairs write permissions; more information below.

This project was made to be used on jailbroken iOS devices, as the app needed to read and write files. Also, in order to manipulate .chr files or even add mods, you need to view the directories of the application, which is only available for jailbroken handsets.

If you just install the deb or iPA, there will be a traceback where DDLC cannot create new files or delete the .chr files. If you changed permissions on the base folder using chmod 777, it will allow write access. After doing this, no tracebacks were encountered.

Tested on iPad 5th generation and iPhone 12 Pro, both on iOS 14.3. Jailbreaks used were Checkra1n 0.12.4 and Taurine 1.04, respectively. The deb installs an app as /Applications/DDLCsteamiOS/. There you can find game files in base/.

Theoretically, mods for DDLC can be loaded by placing mod .rpa files into the base/game folder, like you would on Steam games. The mods "Fruits of the Literature Club", "Exit Music", "DDLC Purist Mod", "Fallen Angel", and "Monika After Story" were tested this way. They also work with the DDLCRMM shortcut linked above. Make sure to delete persistent save files in var/mobile/Containers/data/Applications before starting new mods. Mods that require custom libraries like the Just Yuri mod should not work, however.

Releases should have a deb file compiled from this project, which can be installed using filza file manager or another package manager.

