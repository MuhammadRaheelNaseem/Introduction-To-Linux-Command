
## **Introduction to Linux Commands**

The Linux command line (or shell) is a powerful tool that allows users to interact with the system by typing commands. Whether you're a system administrator, developer, or just exploring Linux, mastering these basic commands is crucial. In this lecture, we will cover the most commonly used Linux commands, explaining their functionality and syntax with practical examples.

---

### **1. `ls` - List Directory Contents**

The `ls` command lists the files and directories in the current working directory.

- **Syntax:**
  ```bash
  ls
  ```
- **Example:**
  ```bash
  ls /home/user/Documents
  ```
- **Options:**
  - `-a`: Displays all files, including hidden ones (files starting with a dot).
    ```bash
    ls -a
    ```
  - `-l`: Lists files in long format, showing permissions, owner, and size.
    ```bash
    ls -l
    ```

---

### **2. `mkdir` - Make Directories**

The `mkdir` command creates new directories.

- **Syntax:**
  ```bash
  mkdir directory_name
  ```
- **Example:**
  ```bash
  mkdir new_project
  ```
- **Options:**
  - `-p`: Creates parent directories as needed.
    ```bash
    mkdir -p new_project/sub_folder
    ```

---

### **3. `clear` - Clear the Terminal Screen**

The `clear` command clears the terminal window, making the screen clean and easier to work with.

- **Syntax:**
  ```bash
  clear
  ```

---

### **4. `cd` - Change Directory**

The `cd` command allows you to navigate through directories in the file system.

- **Syntax:**
  ```bash
  cd directory_name
  ```
- **Examples:**
  - Move to the home directory:
    ```bash
    cd ~
    ```
  - Move up one directory level:
    ```bash
    cd ..
    ```
  - Move to a specific directory:
    ```bash
    cd /home/user/Documents
    ```

---

### **5. `nano` - Text Editor**

`nano` is a simple text editor that allows you to create and edit files from the command line.

- **Syntax:**
  ```bash
  nano filename
  ```
- **Example:**
  ```bash
  nano notes.txt
  ```
- **Basic Usage:**
  - Type text to create or edit the file.
  - Save and exit: `Ctrl+X`, then press `Y` and `Enter`.
  - Exit without saving: `Ctrl+X`, then press `N`.

---

### **6. `ping` - Check Network Connectivity**

The `ping` command tests the connection between your machine and a remote server.

- **Syntax:**
  ```bash
  ping hostname_or_ip
  ```
- **Example:**
  ```bash
  ping google.com
  ```
- Press `Ctrl+C` to stop the `ping` test.

---

### **7. `cat` - Concatenate and Display File Contents**

The `cat` command displays the contents of a file or concatenates multiple files.

- **Syntax:**
  ```bash
  cat filename
  ```
- **Examples:**
  - Display the contents of a file:
    ```bash
    cat notes.txt
    ```
  - Concatenate two files and display them:
    ```bash
    cat file1.txt file2.txt
    ```

---

### **8. `who` - Show Who is Logged In**

The `who` command displays a list of users currently logged into the system.

- **Syntax:**
  ```bash
  who
  ```

---

### **9. `hostname` - Display Hostname**

The `hostname` command shows the name of the current system.

- **Syntax:**
  ```bash
  hostname
  ```

---

### **10. `pwd` - Print Working Directory**

The `pwd` command displays the full path of the current working directory.

- **Syntax:**
  ```bash
  pwd
  ```

---

### **11. `rm` - Remove Files and Directories**

The `rm` command removes files or directories.

- **Syntax:**
  ```bash
  rm filename
  ```
- **Example:**
  ```bash
  rm notes.txt
  ```
- **Options:**
  - `-r`: Recursively remove directories and their contents.
    ```bash
    rm -r folder_name
    ```

---

### **12. `cp` - Copy Files and Directories**

The `cp` command copies files or directories from one location to another.

- **Syntax:**
  ```bash
  cp source destination
  ```
- **Example:**
  ```bash
  cp file1.txt /home/user/Documents/
  ```

---

### **13. `mv` - Move or Rename Files and Directories**

The `mv` command moves files or directories, or renames them.

- **Syntax:**
  ```bash
  mv source destination
  ```
- **Examples:**
  - Move a file:
    ```bash
    mv file.txt /home/user/Documents/
    ```
  - Rename a file:
    ```bash
    mv oldname.txt newname.txt
    ```

---

### **14. `chmod` - Change File Permissions**

The `chmod` command modifies the permissions of files or directories.

- **Syntax:**
  ```bash
  chmod permissions filename
  ```
- **Example:**
  ```bash
  chmod 755 script.sh
  ```
  Here, `755` gives the owner full permissions and read/execute permissions to others.

---

### **15. `top` - Display Running Processes**

The `top` command shows the currently running processes and their system resource usage.

- **Syntax:**
  ```bash
  top
  ```

---

### **16. `sudo` - Superuser Privileges**

The `sudo` command allows a permitted user to run a command as the superuser or another user.

- **Syntax:**
  ```bash
  sudo command
  ```
- **Example:**
  ```bash
  sudo apt-get update
  ```

---

### **17. `echo` - Display a Line of Text**

The `echo` command outputs the provided text or variables.

- **Syntax:**
  ```bash
  echo "Your message here"
  ```
- **Example:**
  ```bash
  echo "Hello, world!"
  ```

---

### **18. `history` - View Command History**

The `history` command displays a list of previously used commands.

- **Syntax:**
  ```bash
  history
  ```

---

### **19. `df` - Disk Space Usage**

The `df` command shows the disk space usage of file systems.

- **Syntax:**
  ```bash
  df
  ```
- **Example:**
  ```bash
  df -h
  ```
  The `-h` option shows the output in human-readable format (e.g., MB, GB).

---

### **20. `free` - Memory Usage**

The `free` command displays the amount of free and used memory in the system.

- **Syntax:**
  ```bash
  free
  ```
- **Example:**
  ```bash
  free -h
  ```
  The `-h` option shows the output in human-readable format.

---


## *Intermediate Command*

---

### **1. `apt-get` - Package Management**

The `apt-get` command installs, updates, or removes packages on Debian-based systems (like Ubuntu).

- **Syntax:**
  ```bash
  sudo apt-get install package_name
  ```
- **Example:**
  ```bash
  sudo apt-get install vim
  ```

---

### **2. `du` - Disk Usage**

The `du` command shows the disk usage of files and directories.

- **Syntax:**
  ```bash
  du
  ```
- **Example:**
  ```bash
  du -h /home/user
  ```
  The `-h` flag displays sizes in a human-readable format.

---

### **3. `ps` - Process Status**

The `ps` command lists running processes.

- **Syntax:**
  ```bash
  ps
  ```
- **Options:**
  - `aux`: Displays all processes in a user-friendly format.
    ```bash
    ps aux
    ```

---

### **4. `kill` - Terminate Processes**

The `kill` command sends signals to terminate a process using its process ID (PID).

- **Syntax:**
  ```bash
  kill PID
  ```
- **Example:**
  ```bash
  kill 1234
  ```

---

### **5. `zip` - Compress Files**

The `zip` command compresses files into a .zip archive.

- **Syntax:**
  ```bash
  zip archive_name.zip file1 file2
  ```

---

### **6. `unzip` - Extract Zip Files**

The `unzip` command extracts files from a .zip archive.

- **Syntax:**
  ```bash
  unzip archive_name.zip
  ```

---

### **7. `chmod` - Change File Permissions**

The `chmod` command modifies file permissions.

- **Syntax:**
  ```bash
  chmod 755 file_name
  ```
  The `755` sets read/write/execute permissions for the owner, and read/execute for others.

---

### **8. `chown` - Change File Ownership**

The `chown` command changes the ownership of a file or directory.

- **Syntax:**
  ```bash
  sudo chown owner:group filename
  ```
- **Example:**
  ```bash
  sudo chown user:group file.txt
  ```

---

### **9. `find` - Search for Files**

The `find` command searches for files in a directory hierarchy.

- **Syntax:**
  ```bash
  find /path -name filename
  ```
- **Example:**
  ```bash
  find /home/user -name notes.txt
  ```

---

### **10. `locate` - Quickly Find Files**

The `locate` command finds files based on the file database, offering faster results than `find`.

- **Syntax:**
  ```bash
  locate filename
  ```

---

### **11. `df` - Disk Space Information**

The `df` command displays the disk space usage of mounted file systems.

- **Syntax:**
  ```bash
  df -h
  ```
  The `-h` flag shows the output in human-readable format.

---

### **12. `ln` - Create Symbolic Links**

The `ln` command creates hard or symbolic (soft) links between files.

- **Syntax (symbolic link):**
  ```bash
  ln -s source_file link_name
  ```

---

### **13. `alias` - Create Aliases**

The `alias` command creates a shortcut for a command.

- **Syntax:**
  ```bash
  alias short_name='command'
  ```
- **Example:**
  ```bash
  alias ll='ls -l'
  ```

---

### **14. `scp` - Secure File Copy**

The `scp` command copies files between hosts over SSH.

- **Syntax:**
  ```bash
  scp file.txt user@remote:/path/to/destination
  ```

---

### **15. `wget` - Download Files from the Internet**

The `wget` command downloads files from the web.

- **Syntax:**
  ```bash
  wget URL
  ```

---

### **16. `curl` - Transfer Data to or from a Server**

The `curl` command fetches data from or sends data to a server using various protocols.

- **Syntax:**
  ```bash
  curl URL
  ```

---

### **17. `df` - Disk Space Usage**

The `df` command displays information about the disk space used and available.

- **Syntax:**
  ```bash
  df -h
  ```

---

### **18. `top` - Monitor System Processes**

The `top` command displays real-time system processes, CPU usage, and memory usage.

- **Syntax:**
  ```bash
  top
  ```

---

### **19. `uptime` - System Uptime**

The `uptime` command shows how long the system has been running.

- **Syntax:**
  ```bash
  uptime
  ```

---

### **20. `history` - View Command History**

The `history` command displays a list of previously executed commands.

- **Syntax:**
  ```bash
  history
  ```

---

### **21. `sort` - Sort Lines of Text Files**

The `sort` command sorts the lines of a text file.

- **Syntax:**
  ```bash
  sort filename.txt
  ```

---

### **22. `uniq` - Report or Omit Repeated Lines**

The `uniq` command filters out repeated lines in a file.

- **Syntax:**
  ```bash
  uniq filename.txt
  ```

---

### **23. `tr` - Translate or Delete Characters**

The `tr` command translates or deletes characters from the input.

- **Syntax:**
  ```bash
  tr 'abc' '123'
  ```

---

### **24. `tar` - Archive Files**

The `tar` command is used to compress and extract `.tar` archives.

- **Syntax:**
  ```bash
  tar -czvf archive_name.tar.gz /path/to/files
  ```
  To extract:
  ```bash
  tar -xzvf archive_name.tar.gz
  ```

---

### **25. `head` - Display the First Lines of a File**

The `head` command shows the first 10 lines of a file by default.

- **Syntax:**
  ```bash
  head filename.txt
  ```

---

### **26. `tail` - Display the Last Lines of a File**

The `tail` command shows the last 10 lines of a file by default.

- **Syntax:**
  ```bash
  tail filename.txt
  ```

---

### **27. `tee` - Read and Write to Multiple Outputs**

The `tee` command reads from standard input and writes to standard output and files simultaneously.

- **Syntax:**
  ```bash
  command | tee output_file
  ```

---

### **28. `jobs` - List Background Jobs**

The `jobs` command displays all active background jobs.

- **Syntax:**
  ```bash
  jobs
  ```

---

### **29. `bg` - Run Jobs in the Background**

The `bg` command resumes a suspended job and runs it in the background.

- **Syntax:**
  ```bash
  bg job_number
  ```

---

### **30. `fg` - Bring Jobs to the Foreground**

The `fg` command brings a background job to the foreground.

- **Syntax:**
  ```bash
  fg job_number
  ```

---

### **Advance Command**

---

### **1. `echo` - Print Text to the Terminal**

The `echo` command outputs the given string or variable to the terminal.

- **Syntax:**
  ```bash
  echo "Hello, World!"
  ```

---

### **2. `alias` - Create Shortcut Commands**

The `alias` command creates an alias or shortcut for a command.

- **Syntax:**
  ```bash
  alias newcommand='existingcommand'
  ```
- **Example:**
  ```bash
  alias ll='ls -l'
  ```

---

### **3. `unalias` - Remove Alias**

The `unalias` command removes an existing alias.

- **Syntax:**
  ```bash
  unalias alias_name
  ```

---

### **4. `basename` - Strip Directory and Suffix from Filenames**

The `basename` command returns the filename by removing the directory path.

- **Syntax:**
  ```bash
  basename /path/to/file
  ```

---

### **5. `dirname` - Get Directory Name from a Path**

The `dirname` command returns the directory part of a file path.

- **Syntax:**
  ```bash
  dirname /path/to/file
  ```

---

### **6. `uname` - Print System Information**

The `uname` command shows system information, including kernel name, version, and architecture.

- **Syntax:**
  ```bash
  uname -a
  ```

---

### **7. `date` - Display or Set System Date and Time**

The `date` command displays the current date and time or sets the system date.

- **Syntax:**
  ```bash
  date
  ```

---

### **8. `cal` - Display a Calendar**

The `cal` command displays a simple calendar for the current month.

- **Syntax:**
  ```bash
  cal
  ```

---

### **9. `dd` - Convert and Copy Files**

The `dd` command is used to copy and convert files, especially for creating bootable drives.

- **Syntax:**
  ```bash
  dd if=input_file of=output_file
  ```
- **Example:**
  ```bash
  dd if=/dev/sda of=backup.img
  ```

---

### **10. `df` - Disk Space Usage**

The `df` command displays information about the file system disk space usage.

- **Syntax:**
  ```bash
  df -h
  ```
  The `-h` option shows sizes in human-readable format.

---

### **11. `du` - Estimate File Space Usage**

The `du` command estimates the file or directory space usage.

- **Syntax:**
  ```bash
  du -h /path
  ```

---

### **12. `free` - Display Memory Usage**

The `free` command displays the amount of free and used memory in the system.

- **Syntax:**
  ```bash
  free -h
  ```

---

### **13. `env` - Display Environment Variables**

The `env` command displays all the environment variables.

- **Syntax:**
  ```bash
  env
  ```

---

### **14. `export` - Set Environment Variables**

The `export` command sets environment variables.

- **Syntax:**
  ```bash
  export VAR_NAME=value
  ```

---

### **15. `unset` - Remove Environment Variables**

The `unset` command deletes an environment variable.

- **Syntax:**
  ```bash
  unset VAR_NAME
  ```

---

### **16. `id` - Print User and Group Information**

The `id` command prints user and group IDs.

- **Syntax:**
  ```bash
  id
  ```

---

### **17. `groups` - Show User's Groups**

The `groups` command shows the groups that the current user is part of.

- **Syntax:**
  ```bash
  groups
  ```

---

### **18. `which` - Show Full Path of Commands**

The `which` command shows the full path of shell commands.

- **Syntax:**
  ```bash
  which command
  ```

---

### **19. `type` - Display Command Type**

The `type` command tells you whether a command is an alias, a shell function, or a built-in command.

- **Syntax:**
  ```bash
  type command
  ```

---

### **20. `whereis` - Locate Binary, Source, and Manual Pages**

The `whereis` command locates the binary, source code, and manual page of a command.

- **Syntax:**
  ```bash
  whereis command
  ```

---

### **21. `whatis` - Brief Description of Commands**

The `whatis` command provides a brief description of a command.

- **Syntax:**
  ```bash
  whatis command
  ```

---

### **22. `uptime` - Show System Uptime**

The `uptime` command shows how long the system has been running, as well as the load averages.

- **Syntax:**
  ```bash
  uptime
  ```

---

### **23. `last` - Show Login History**

The `last` command shows the login history of users.

- **Syntax:**
  ```bash
  last
  ```

---

### **24. `shutdown` - Shut Down the System**

The `shutdown` command powers off the system at a specified time.

- **Syntax:**
  ```bash
  sudo shutdown
  ```
- **Example:**
  To shut down immediately:
  ```bash
  sudo shutdown now
  ```

---

### **25. `reboot` - Reboot the System**

The `reboot` command reboots the system.

- **Syntax:**
  ```bash
  sudo reboot
  ```

---

### **26. `df` - Show Disk Space**

The `df` command displays information about available and used disk space on file systems.

- **Syntax:**
  ```bash
  df -h
  ```

---

### **27. `tar` - Archive Files**

The `tar` command is used to create or extract tar archives.

- **Syntax:**
  ```bash
  tar -cvf archive_name.tar /path/to/directory
  ```
  To extract:
  ```bash
  tar -xvf archive_name.tar
  ```

---

### **28. `gzip` - Compress Files**

The `gzip` command compresses files.

- **Syntax:**
  ```bash
  gzip filename
  ```

---

### **29. `gunzip` - Decompress Files**

The `gunzip` command decompresses `.gz` files created by `gzip`.

- **Syntax:**
  ```bash
  gunzip filename.gz
  ```

---

### **30. `file` - Determine File Type**

The `file` command tells the type of a file.

- **Syntax:**
  ```bash
  file filename
  ```

---

## **Conclusion**

These basic Linux commands form the foundation of interacting with the system from the terminal. Mastering them is essential for anyone who wants to use Linux efficiently. Remember, practice is key to becoming proficient, and many commands have additional options that can be explored using `man` or `--help`.
