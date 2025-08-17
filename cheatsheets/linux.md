# Linux

Linux is a Unix-like, open-source operating system kernel that serves as the core of countless distributions. It manages hardware resources, provides essential services for software, and enables multi-user, multitasking operation with robust security.

---

### **Documentation and Help**

| Command           | Description                                            |
| ----------------- | ------------------------------------------------------ |
| man [command]    | Displays the complete manual of the specified command. |
| [command] --help | Shows a quick usage summary and command options.       |

---

### **User and Permissions**

| Command                      | Description                                                      |
| ---------------------------- | ---------------------------------------------------------------- |
| whoami                       | Returns the current user’s name.                                 |
| su                           | Switches to superuser (root) or another user; requires password. |
| sudo [command]              | Executes the command with administrative privileges.             |
| passwd                       | Changes the current user’s password.                             |
| useradd [username]          | Creates a new user in the system.                                |
| groupadd [groupname]        | Creates a new group in the system.                               |
| usermod -aG [group] [user] | Adds the user to an existing group.                              |

---

### **File Navigation and Management**

| Command                     | Description                                           |
| --------------------------- | ----------------------------------------------------- |
| ls                          | Lists files and directories in the current directory. |
| pwd                         | Shows the full path of the current directory.         |
| cd [directory]              | Changes to the specified directory.                   |
| mkdir [directory]           | Creates a new directory.                              |
| rm [file]                   | Deletes a file.                                       |
| cp [source] [destination]   | Copies a file or directory.                           |
| mv [source] [destination]   | Moves or renames a file or directory.                 |
| touch [file]                | Creates an empty file or updates its timestamp.       |
| cat [file]                  | displays the contents of files in the terminal.       |
| nano [file]                 | Opens the file in the nano text editor.               |
| cat [file]                  | Displays the entire content of a file.                |
| head [file]                 | Shows the first 10 lines of a file.                   |
| tail [file]                 | Shows the last 10 lines of a file.                    |
| less [file]                 | Displays file content in a paginated way.             |
| locate [file]               | Quickly finds the file path.                          |
| grep "[term]" [file]        | Searches for a specific term inside a file.           |

---

### **File Compression and Transfer**

| Command         | Description                                                                                       |
| --------------- | ------------------------------------------------------------------------------------------------- |
| unzip [file]   | Extracts a `.zip` archive.                                                                        |
| tar -xf [file] | Extracts files from a `.tar` archive.                                                             |
| wget [url]     | Downloads a file from the internet via HTTP/HTTPS.                                                |
| curl [url]     | Transfers data from or to a server using various protocols. Can download or upload data flexibly. |

---

### **Processes**

| Command                | Description                                   |
| ---------------------- | --------------------------------------------- |
| top                    | Shows real-time processes and resource usage. |
| ps                     | Lists current session processes.              |
| kill [PID]            | Terminates the process with the specified ID. |
| killall [processname] | Terminates all processes with the given name. |

---

### **Remote Access and Secure Copy**

| Command                        | Description                                |
| ------------------------------ | ------------------------------------------ |
| ssh [user]@[ip]                | Connects to a remote host via SSH.         |
| scp [file] [user]@[ip]:[path] | Copies a file to another machine over SSH. |

---

### **Volumes, Disks and Filesystems**

| Command                               | Description                                            |
| ------------------------------------- | ------------------------------------------------------ |
| df -h                                 | Shows disk space usage of all mounted volumes.         |
| du -h [directory]                    | Shows disk space usage of a directory.                 |
| mount [/dev/device] [/mount_point] | Mounts the device to the filesystem mount point.       |
| umount [/mount_point]               | Unmounts the volume from the specified mount point.    |
| lsblk                                 | Lists all connected block devices (disks, partitions). |
| blkid                                 | Shows UUIDs and filesystem types of devices.           |
| fdisk [/dev/device]                  | Manages disk partitions interactively.                 |
| parted [/dev/device]                 | Creates and manipulates partitions.                    |
| mkfs.[type] [/dev/partition]        | Formats the partition with the specified filesystem.   |
| fsck [/dev/partition]                | Checks and repairs filesystem errors on the partition. |

---
