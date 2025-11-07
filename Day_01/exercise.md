### Day 01

- What is the Linux kernel, and how does it differ from a Linux distribution?
Ans. Kernel is part of the OS package. It is a piece of software(low level program) that handles:
    1. Hardware interaction.
    2. Device drivers
    3. Memory allocation
    4. Security
    5. System Calls
It is not shell. 
Linux distribution also includes: GNU, package managers, applicationsand gnome like tools for HUI.


- Explain kernel space vs. user space. Why is this separation important for system security and stability?
Ans. Kernel space and user space are isolations created so that things running in user space do not have access to kernel space. Within kernel space it has unrestricted access to system resources.
When applications are run within the User space they use the system resources and get some kind of access to kernel space via system calls.

- Name three popular Linux distributions and their typical use cases in a cloud environment.
Ans.1. Arch: known for being very customizable
    2. Ubuntu/Debian: used to get started or very easy learning curve.
    3. Parrot/Kali: used for security purpose.

- How do package managers like apt and yum work? Why are they essential for DevOps workflows?
Ans. apt and yum have a file list.d which points to the remote sources where the latest indexes of the packages are updates. And using the update commands the local packages and binaries have their index updated. 
    - They are then upgraded to the latest version using upgrade command.
    - To add a new package that doesnt exist install command is used and remove to remove.
    - They are essential for devops workflow because of the automation and convenience it provides: dependency mgmt, security updates, reproducibility etc 

- In a production SRE role, why might you prefer Linux over Windows for server infrastructure?
Ans. 
    - Easier automation (scripting)
    - Cloud native
    - Stable(avoids forced updates)
    - Open source, lightweight

- What is the role of the GNU Project in the Linux ecosystem? Why is the full name often "GNU/Linux"?
Ans. GNU provides the essential tooling, libraries and utilities like bash, coreutils and glibc. Kernel alone cannot be considered as complete OS. Hence the name GNU/Linux

- How would you check the kernel version on a Linux instance, and why might a cloud provider use an older version?
Ans. <uname -r> can be used to check the kernel version.
Older versions are widely tested and easier to maintain.