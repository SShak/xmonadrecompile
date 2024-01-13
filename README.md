This file needs to placed in /etc/pacman.d/hooks in your root directory.
When upgrading the system haskell files may be updated and you will need to recompile xmonad before reboot or shutdown. If you do not, xmonad may not start.
This script will force recompile Xmonad after a system upgrade.

You will also need to edit you /etc/pacman.conf file.
Under General Options uncomment HookDir and set the file path to /etc/pacman.d/hooks/ if it is not alread set.

Now you don't need to worry about borking your system if you forget to recompile! 

p.s. While you are in pacman.conf st your ParrallelDownloads = 5, because if you don't....what are you really doing with your life?
