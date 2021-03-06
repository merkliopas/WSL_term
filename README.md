# Terminal for WSL

Basically, this is an automated implementation of terminal (terminator) emulator for WSL based on [this](https://blog.ropnop.com/configuring-a-pretty-and-usable-terminal-emulator-for-wsl/) guide. Assumes that WSL is already installed, you have sudo rights for installing terminator (just run `sudo terminator.sh` in bash) and that BITS Transfer is enabled in poweshell.

If so, just execute `install.ps1` and it will download VcXsrv, ask for confirmation to install it, and produce a shortcut to terminator on desktop. Afterwards, restart your PC to make sure the start-up job of launching X-Server is initiated.

Terminator.sh installs terminator GTK3, because I found it works better on WSL and X-Server, however, many dependencies are required for it to run. If you do not have sudo rights to prepare your system for terminator GTK3 you can install regular terminator and not run terminator.sh. However, it might have problems with full screen.

![screenshot](icon/screenshot.JPG?raw=true)
