# Linux Distro Installation

This document describes the installation of a Linux distribution using **Windows Subsystem for Linux (WSL)**.  
The goal is to create a safe and controlled learning environment for practicing Linux fundamentals without modifying the host operating system.

WSL is ideal for beginners because it allows running a real Linux environment directly on Windows, making it easy to experiment, learn, and reset if needed.

# Installation steps
1. Search for Power Shell in your start menu for windows : press Windows key on your keyboard and then search PowerShell.
2. Run Power Shell as Administartor.
3. Now you should be able to see a terminal, in this terminal type the following command: wsl --install.
4. Type wsl in your terminal to check if it is installed.
5. After everything is installed you can check what Linux distros are available by typing the command: wsl.exe --list --online.
6. From that list you can choose a distro with wsl.exe --install [Distro name] !!Do not use the square bracket
7. Congrats! Now you installed your first Linux distro. Now you can run the distro by searching for it in the start menu on Windows.
