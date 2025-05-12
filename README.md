# cp_-r_emulator

This script is effectively an emulation of the "cp -r <source> <target>" terminal command. This is the recursive copy terminal command.

The calling format for this script is "./copy_and_remove.bash <sourceDirectory> <targetDirectory>


How it works:
Call a recursive function which: 
	- a) Scans the source directory for all files and directories
	- b) When a file is found, it creates a similar file in the target directory 
	- c) When a directory is found, it creates a similar directory in the target directory and:
	- d) Recursively calls itself to the sub-directory
