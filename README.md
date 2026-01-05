# Linux Command Line Lab Assignment (Modules 1–4)

This repository contains my graded Linux Command Line Interface (CLI) laboratory assignment.  
The objective of this lab was to demonstrate hands-on understanding of Linux user environments, file systems, links, disk usage, and system monitoring tools using real command execution.

Each question is organized in its own folder and contains:
- The exact commands executed and the outputs 
- Screenshots of the terminal showing execution
- Files created during the tasks
- A written explanation after for every command used, as required

All commands were executed using my own Linux user account, and the outputs reflect my personal system state.

---

## Repository Structure

The repository is organized as follows:

Question1/ – User identity, environment verification, and basic Linux commands  
Question2/ – File and directory management  
Question3/ – Links, inodes, and disk usage  
Question4/ – System monitoring, processes, memory, and disk inspection  

Each folder contains: 
- `explanations.txt` – 1–2 sentence explanation for every command  
- Screenshots folder – Proof of command execution  
- Files created as part of the tasks  

---

# Question 1 — Linux Environment Verification

In this section, I verified my Linux user environment and ensured that the system was functioning correctly.

I checked my logged-in identity and group memberships to confirm that I was operating under my own user account. I then verified my working directory and listed files to understand my current workspace.

A confirmation file (`user_info.txt`) was created to demonstrate file creation and writing, and I validated its integrity by counting its characters. I also accessed the documentation for the `mkdir` command to understand how directory creation works, learning about useful options such as creating parent directories automatically.

Additionally, I inspected my home directory, searched logs for administrative activity, checked the Linux kernel version, tested network connectivity using ICMP packets, and examined system uptime.  
These steps confirmed that the system was operational, connected to the internet, and running a valid Linux kernel.

This section taught me how to quickly validate whether a Linux system is usable and healthy when logging in for the first time.

---

# Question 2 — File and Directory Management

This section focused on managing files and directories in a Linux environment.

I created a dedicated workspace in my home directory, added files to it, wrote content into those files, and verified their ownership and permissions. I then duplicated files, renamed directories, created subdirectories for organization, and moved files into appropriate locations.

Finally, I displayed the full directory structure recursively and verified the absolute path of a file after it was moved.  
This exercise showed how Linux uses paths, directories, and file metadata to organize data.

From this task, I learned how to structure project folders cleanly, track file locations, and use Linux commands to manage file systems efficiently.

---

# Question 3 — Links, Inodes, and Disk Usage

This section explored how Linux manages files internally.

I created a file and then made both a hard link and a symbolic link to it. By examining inode numbers, I observed that the original file and the hard link shared the same inode, proving that they refer to the same physical data on disk, while the symbolic link had a different inode because it only stores a file path.

I inspected file metadata, measured disk usage of my home directory, and listed file sizes in human-readable format. I also deleted the symbolic link to demonstrate that removing a soft link does not delete the original file.

Finally, I used `du` and `df` to understand how disk space is consumed and how much space is available on the filesystem.  
This taught me the difference between storage usage inside directories and overall disk capacity.

---

# Question 4 — System Monitoring and Resource Management

This section focused on understanding how a Linux system runs in real time.

I checked system uptime, listed all processes running under my user account, and used process monitoring tools to identify which process was using the most CPU. I launched a background process and confirmed that it was running, then changed its priority using `renice`.

I also monitored memory usage, checked disk space of the filesystem containing my home directory, and identified the shell I was using. System information was redirected into a file (`system_report.txt`) to demonstrate output redirection.

Finally, I used `ncdu` to visually inspect how disk space is distributed across directories.

This section showed how Linux manages CPU, memory, storage, and processes, and how administrators can inspect and control system performance.

---

## What I Learned

Through this lab, I gained hands-on experience with:
- Linux user identities and permissions
- File and directory management
- Links, inodes, and file systems
- Disk usage and storage analysis
- Process management and system monitoring
- Command documentation and output redirection

Rather than just memorizing commands, this lab taught me how Linux actually works behind the scenes — how files are stored, how processes run, and how system resources are tracked; basically how it feels using it for real-world applications rather than just playing around with commands for the sake of it.

This practical experience is essential for working with real servers and Linux-based systems in engineering and computing environments.
