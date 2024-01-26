# CMD Cheat Sheet

---
## **UNDER CONSTRUCTION**
---

A cheat sheet for CMD commands.

#

## **<u id="cmd-commands">CMD Commands</u>** [source&nearr;](https://ss64.com/nt/)

#### - Open via Run dialog box - Windows Key + R, then type cmd

#### - Open via File Explorer - Ctrl + l, then type cmd

#### - Open via File Explorer - Shift + Right-click on a folder, then choose Open command window here

#### - Drag and drop a folder into the command window to type the path

| Command       | Description                                      |
| ------------- | ------------------------------------------------ |
| `F7`          | Display command history                          |
| `F1`          | Copy previous command                            |
| `\| clip`     | Copy command output to clipboard                 |
| `>`           | Redirect command output to file                  |
| `>>`          | Append command output to file                    |
| `&&`          | Run multiple commands on one line if previous ok |
| `&`           | Run multiple commands on one line                |
| `^`           | Escape character                                 |
| `\|\|`        | Run command if previous command fails            |
| `/?`          | Help                                             |
| `cls`         | Clear Screen                                     |
| `cd`          | Change Directory                                 |
| `cd ..`       | Change Directory to parent folder                |
| `cd \`        | Change Directory to root folder                  |
| `cd /d`       | Change Directory to a specific drive             |
| `md`          | Make Directory                                   |
| `rd`          | Remove Directory                                 |
| `del`         | Delete file                                      |
| `del /f`      | Force delete file                                |
| `del /q`      | Quiet mode, do not ask if ok to delete on global |
| `dir`         | List files and folders                           |
| `dir /a`      | List all files and folders                       |
| `copy`        | Copy file                                        |
| `move`        | Move file                                        |
| `ren`         | Rename file                                      |
| `type`        | Display file contents                            |
| `echo`        | Display message                                  |
| `start`       | Start program                                    |
| `tasklist`    | List running processes                           |
| `taskkill`    | Kill process                                     |
| `shutdown`    | Shutdown computer                                |
| `shutdown /r` | Restart computer                                 |

## Command History

```Bash
F7 # Display command history
F1 # Copy previous command
```

## Navigation in CMD

```Bash
cd # list current directory
cd [folder] # Change Directory
cd .. # Change Directory to parent folder
cd \  # Change Directory to root folder
cd /[drive-letter] # Change Directory to a specific drive
dir # List files and folders
dir /a # List all files and folders
dir /s # List all files and folders in subfolders
tree # List all files and folders in current directory and subdirectories
tree [folder] # List all files and folders in a specific directory and subdirectories
tree /f # List all files and folders in current directory and subdirectories with file names
tree /a # List all files and folders in current directory and subdirectories with file names and hidden files
tree /a /f # List all files and folders in current directory and subdirectories with file names, hidden files, and file sizes
tree /a /f > [file-name] # List all files and folders in current directory and subdirectories with file names, hidden files, and file sizes, and save to a file
```

## Creating Directories

```Bash
md [folder] # Make Directory
md [folder1] [folder2] # Make Multiple Directories
md [folder]\[subfolder] # Make Directory and Subdirectory
md [folder]\[subfolder1] [folder]\[subfolder2] # Make Multiple Directories and Subdirectories
```

## Move and Copy Directories

```Bash
copy [folder] [new-folder] # Copy Directory
copy [folder] [new-folder]\[subfolder] # Copy Directory and Subdirectory
copy [folder]\[subfolder] [new-folder]\[subfolder] # Copy Subdirectory
move [folder] [new-folder] # Move Directory
move [folder] [new-folder]\[subfolder] # Move Directory and Subdirectory
move [folder]\[subfolder] [new-folder]\[subfolder] # Move Subdirectory
```

## Renaming Directories

```Bash
ren [folder] [new-folder] # Rename Directory
ren [folder]\[subfolder] [new-folder]\[subfolder] # Rename Subdirectory
```

## Deleting Directories

```Bash
rd [folder] # Remove Directory
rd [folder] /s # Remove Directory and all files and subdirectories
rd [folder] /s /q # Remove Directory and all files and subdirectories without asking for confirmation
```

## Creating Files

```Bash
copy nul [file-name] # Create Empty File
copy con [file-name] # Create File and Enter Text
echo. > [file-name] # Create File
echo [text] > [file-name] # Create File and Enter Text
type nul > [file-name] # Create File
fsutil file createnew [file-name] [file-size] # Create File with Size
```

## Move and Copying Files

```Bash
copy [file-name] [new-file-name] # Copy File
copy [file-name] [new-folder]\[file-name] # Copy File to Folder
copy [file-name] [new-folder]\[new-file-name] # Copy File to Folder and Rename
move [file-name] [new-file-name] # Move File
move [file-name] [new-folder]\[file-name] # Move File to Folder
move [file-name] [new-folder]\[new-file-name] # Move File to Folder and Rename
```

## Renaming Files

```Bash
ren [file-name] [new-file-name] # Rename File
```

## Deleting Files

```Bash
del [file-name] # Delete File
del /f [file-name] # Force Delete File
del /q [file-name] # Quiet Delete File
del [folder]\[file-name] # Delete File in Folder
del [folder]\[subfolder]\[file-name] # Delete File in Subfolder
```

## Reading Files

```Bash
type [file-name] # Display File Contents
type [file-name] \| clip # Display File Contents and Copy to Clipboard
type [file-name] \| [command] # Display File Contents and Pipe to Command
type [file-name] \| [command] > [file-name] # Display File Contents and Pipe to Command and Save to File
type [file-name] \| [command] >> [file-name] # Display File Contents and Pipe to Command and Append to File
findstr /n "^" [file-name] # Display File Contents with Line Numbers
```

## Standard Input and Output

```Bash
echo [text] # Display Text
echo [text] > [file-name] # Display Text and Save to File
echo [text] >> [file-name] # Display Text and Append to File
echo [text] \| clip # Display Text and Copy to Clipboard
echo [text] \| [command] # Display Text and Pipe to Command
echo [text] \| [command] > [file-name] # Display Text and Pipe to Command and Save to File
echo [text] \| [command] >> [file-name] # Display Text and Pipe to Command and Append to File
```

## Standard Error

```Bash
[command] 2> [file-name] # Redirect Standard Error to File
[command] 2>> [file-name] # Redirect Standard Error to File and Append
[command] 2>&1 # Redirect Standard Error to Standard Output
[command] 2>&1 > [file-name] # Redirect Standard Error to Standard Output and Save to File
[command] 2>&1 >> [file-name] # Redirect Standard Error to Standard Output and Append to File
```

## File Permissions

| #   | Permission       | Symbol | Binary |
| --- | ---------------- | ------ | ------ |
| 0   | No Access        | -      | 000    |
| 1   | Execute          | X      | 001    |
| 2   | Write            | W      | 010    |
| 4   | Read             | R      | 100    |
| 5   | Read and Execute | RE     | 101    |
| 6   | Read and Write   | RW     | 110    |
| 7   | Full Control     | F      | 111    |

## File Permissions

```Bash
icacls [file-name] # Display File Permissions
icacls [file-name] /grant [user]:[permission] # Grant User Permission
icacls [file-name] /deny [user]:[permission] # Deny User Permission
icacls [file-name] /remove [user] # Remove User Permission
icacls [file-name] /inheritance:e # Enable Inheritance
icacls [file-name] /inheritance:d # Disable Inheritance
icacls [file-name] /reset # Reset Permissions
icacls [file-name] /setowner [user] # Set Owner
```

## File Attributes

```Bash
attrib [file-name] # Display File Attributes
attrib [file-name] +h # Hide File
attrib [file-name] -h # Unhide File
attrib [file-name] +s # Mark File as System File
attrib [file-name] -s # Unmark File as System File
attrib [file-name] +r # Mark File as Read-only
attrib [file-name] -r # Unmark File as Read-only
attrib [file-name] +a # Mark File as Archive
attrib [file-name] -a # Unmark File as Archive
attrib [file-name] +i # Mark File as Not Content Indexed
attrib [file-name] -i # Unmark File as Not Content Indexed
attrib [file-name] +c # Mark File as Compressed
attrib [file-name] -c # Unmark File as Compressed
attrib [file-name] +e # Mark File as Encrypted
attrib [file-name] -e # Unmark File as Encrypted
attrib [file-name] +p # Mark File as Sparse
attrib [file-name] -p # Unmark File as Sparse
attrib [file-name] +u # Mark File as Uncompressed
attrib [file-name] -u # Unmark File as Uncompressed
attrib [file-name] +x # Mark File as No Scrub File
attrib [file-name] -x # Unmark File as No Scrub File
```

## Searching for Files

```Bash
dir [file-name] # Search for File
dir [file-name] /s # Search for File in Subdirectories
dir [file-name] /s /b # Search for File in Subdirectories and Display File Path
dir [file-name] /s /b > [file-name] # Search for File in Subdirectories and Display File Path and Save to File
```

## Searching for Text in Files

```Bash
findstr [text] [file-name] # Search for Text in File
findstr /s [text] [file-name] # Search for Text in File in Subdirectories
findstr /s /n [text] [file-name] # Search for Text in File in Subdirectories and Display Line Numbers
findstr /s /n /i [text] [file-name] # Search for Text in File in Subdirectories and Display Line Numbers and Ignore Case
findstr /s /n /i /m [text] [file-name] # Search for Text in File in Subdirectories and Display Line Numbers and Ignore Case and Display File Names Only
findstr /s /n /i /m /c:"[text]" [file-name] # Search for Text in File in Subdirectories and Display Line Numbers and Ignore Case and Display File Names Only and Search for Exact Text
findstr /s /n /i /m /c:"[text]" [file-name] > [file-name] # Search for Text in File in Subdirectories and Display Line Numbers and Ignore Case and Display File Names Only and Search for Exact Text and Save to File
```

## Symbolic Links

```Bash
mklink [link-name] [target] # Create Symbolic Link
mklink /d [link-name] [target] # Create Symbolic Link to Directory
mklink /h [link-name] [target] # Create Symbolic Link to File
mklink /j [link-name] [target] # Create Symbolic Link to Directory Junction
```

## Compressing Files and Directories

### compact

```Bash
compact [file-name] # Compress File
compact /c [file-name] # Compress File
compact /u [file-name] # Uncompress File
```

## Decompressing Files

### expand

```Bash
expand [file-name] # Decompress File
expand [file-name] [new-file-name] # Decompress File and Rename
```
