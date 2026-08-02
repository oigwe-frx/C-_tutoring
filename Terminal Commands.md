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

You should be able to use the arrow keys or page up and down. When you are ready to exit, just press `q`.

## The `date` Command

Another really simple one is the `date` command, which, surprise, will show you the current date and time.

```bash
  date
```

## File System Navigation

Commands to navigate your file system are very important. You will be using them all the time. You won't remember every single command that you use, but these are the ones that you should remember.

- ```pwd```: Print Working Directory. Displays the absolute path of the folder you are currently in.
- ```ls```: List. Shows the files and folders inside your current directory.
- ```ls -la```: Long List All. Displays detailed file information (permissions, size, date) including hidden files.
- ```cd [directory]```: Change Directory. Moves you into the specified folder.
- ```cd ..```: Move Up. Takes you back to the parent directory of your current location.
- ```cd ~```: Home. Instantly returns you to your user account's home folder.

Of course, you can group flags together. For example, if I want to see more info and view hidden files, I could do `ls -l -a` and even shorten it to `ls -la`.

## Opening a Folder or File

If you want to open a file or a folder in the GUI from your terminal, the command is different depending on the OS.

Mac - `open [dirname]`
Windows - `start [dirname]`
Linux - `xdg-open [dirname]`

You can open folders, files and even URLs

```bash
  open https://www.google.com
```

## File and Folder Management
- ```mkdir [folder_name]```: Make Directory. Creates a new, empty folder.
- ```touch [file_name]```: Touch. Creates a new, empty file (e.g., touch index.html).
- ```cp [source] [destination]```: Copy. Copies a file from one location to another.
- ```mv [source] [destination]```: Move/Rename. Moves a file to a new folder, or renames it if the destination is a new name.
- ```rm [file_name]```: Remove. Deletes a file permanently.
- ```rm -rf [folder_name]```: Force Remove Directory. Deletes a folder and all of its contents completely. Use with extreme caution.

We can also do multiple commands at once with the `&&` operator:

```bash
cd test2 && mkdir test3
```

## Right angle bracket >

This symbol tells the system to output results into whatever you specify next. The target is usually a filename. You can use this symbol by itself to create a new file:

```bash
> [filename]
```

When you are done, hit `ctrl+D`


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

