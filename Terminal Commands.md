# Terminal Commands

Terminal commands are text-based instructions used to navigate your computer, manage files, and run programs without a graphical interface. 
The most essential commands for Unix-based systems (macOS and Linux) focus on file system navigation, file manipulation, and system utilities.
Here is a quick-reference guide to the most common terminal commands.F

## Key Commands & Navigation

Before we look at some common commands, I just want to note a few keyboard commands that are very helpful:

- `Up Arrow`: Will show your last command
- `Down Arrow`: Will show your next command
- `Tab`: Will auto-complete your command
- `Ctrl + L`: Will clear the screen
- `Ctrl + C`: Will cancel a command
- `Ctrl + R`: Will search for a command
- `Ctrl + D`: Will exit the terminal

## Manual Command

On Linux and Mac, the `man` command is used to show the **manual** of any command that you can run in the terminal. So if you wanted to know more about the `ls` command, you could run:

```bash
  man ls
```

Unfortunately, if you are on Windows and using Git Bash, the `man` command is not included, however, you can just type the command that you want to know more about and then `--help` and you will get similar info:

```bash
  ls --help
```

## File System Navigation
- ```pwd```: Print Working Directory. Displays the absolute path of the folder you are currently in.
- ```ls```: List. Shows the files and folders inside your current directory.
- ```ls -la```: Long List All. Displays detailed file information (permissions, size, date) including hidden files.
- ```cd [directory]```: Change Directory. Moves you into the specified folder.
- ```cd ..```: Move Up. Takes you back to the parent directory of your current location.
- ```cd ~```: Home. Instantly returns you to your user account's home folder.


## File and Folder Management
- ```mkdir [folder_name]```: Make Directory. Creates a new, empty folder.
- ```touch [file_name]```: Touch. Creates a new, empty file (e.g., touch index.html).
- ```cp [source] [destination]```: Copy. Copies a file from one location to another.
- ```mv [source] [destination]```: Move/Rename. Moves a file to a new folder, or renames it if the destination is a new name.
- ```rm [file_name]```: Remove. Deletes a file permanently.
- ```rm -rf [folder_name]```: Force Remove Directory. Deletes a folder and all of its contents completely. Use with extreme caution.


## Viewing and Editing Files
- ```cat [file_name]```: Concatenate. Displays the entire text content of a file directly in the terminal.
- ```less [file_name]```: Less. Opens a file for interactive viewing, allowing you to scroll through long texts page by page.
- ```nano [file_name]```: Nano. Opens a simple, beginner-friendly text editor inside the terminal window.
- ```grep "[pattern]" [file]```: Global Regular Expression Print. Searches for specific text fragments inside a file.


## System and Utility Commands
- ```clear```: Clear Screen. Wipes the terminal window clean of old outputs (Keyboard shortcut: Ctrl + L).
- ```history```: History. Displays a numbered list of all commands you have recently executed.
- ```sudo [command]```: SuperUser Do. Runs a command with administrative or root privileges.

## Common Operators
- ```| (Pipe)```: Sends the output of the first command as the input to a second command (e.g., ls | grep "project").
- ```> (Redirect)```: Takes the output of a command and writes it into a new file, overwriting existing content.
- ```>> (Append)```: Takes the output of a command and appends it to the bottom of an existing file.

