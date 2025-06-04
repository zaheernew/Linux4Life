<br><br>

[< Linux4Life](https://github.com/zaheernew/Linux4Life/blob/main/Linux4Life.md)

# Module 3

<br>

## FILE AND DIRECTORY MANAGEMENT

<br>


### FILE SYSTEMS
<table>
    <thead>
    <tr>
        <th> File System</th>
        <th> Use Case</th>
        <th> Key Features</th>
        <th> Pros</th>
        <th> Cons</th>
        <th> Max Volume</th>
        <th> Max File</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> ext4</td>
        <td> General-purpose (default on most Linux distros)</td>
        <td> Journaling, fast mount, delayed allocation</td>
        <td> Stable, mature, widely supported</td>
        <td> No built-in snapshots or advanced features</td>
        <td> 1 EiB</td>
        <td> 16 TiB</td>
    </tr>
    <tr>
        <td> XFS</td>
        <td> Large file handling, media servers, DBs</td>
        <td> High throughput, parallel I/O, online defrag</td>
        <td> Excellent performance with large files</td>
        <td> Poor with many small files, complex tuning</td>
        <td> 8 EiB</td>
        <td> 8 EiB</td>
    </tr>
    <tr>
        <td> Btrfs</td>
        <td> Snapshots, volume management, modern storage</td>
        <td> Snapshots, checksums, compression, RAID</td>
        <td> Advanced features, flexible</td>
        <td> Less stable in some cases, newer than ext4</td>
        <td> 16 EiB</td>
        <td> 16 TiB</td>
    </tr>
    <tr>
        <td> ZFS</td>
        <td> Enterprise-grade, backups, NAS</td>
        <td> End-to-end integrity, RAID-Z, deduplication</td>
        <td> Highly reliable, powerful storage management</td>
        <td> High RAM usage (8GB+), licensing restrictions</td>
        <td> 256 EiB</td>
        <td> 16 TiB</td>
    </tr>
    <tr>
        <td> exFAT / NTFS</td>
        <td> USB drives, dual-boot (Linux ↔ Windows)</td>
        <td> exFAT for flash; NTFS supports journaling</td>
        <td> Cross-platform compatibility</td>
        <td> exFAT lacks journaling; NTFS slower via ntfs-3g</td>
        <td> 128–256 EiB</td>
        <td> 16 TiB</td>
    </tr>
    </tbody>
</table>																								


<br>

### CREATE / REMOVE
<table>
    <thead>
    <tr>
        <th> Command</th>
        <th> Description</th>
        <th> Example</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> touch</td>
        <td> Creates an empty file</td>
        <td> touch notes.txt</td>
    </tr>
    <tr>
        <td> mkdir</td>
        <td> Creates a new directory</td>
        <td> mkdir projects</td>
    </tr>
    <tr>
        <td> rm</td>
        <td> Removes a file</td>
        <td> rm notes.txt</td>
    </tr>
    <tr>
        <td> rm -r</td>
        <td> Removes directory and contents</td>
        <td> rm -r projects</td>
    </tr>
    <tr>
        <td> rmdir</td>
        <td> Removes an empty directory</td>
        <td> rmdir emptyfolder</td>
    </tr>
    </tbody>
</table>												


<br>

### COPY / MOVE
<table>
    <thead>
    <tr>
        <th> Command</th>
        <th> Description</th>
        <th> Example</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> cp</td>
        <td> Copies files or directories</td>
        <td> cp notes.txt backup-notes.txt</td>
    </tr>
    <tr>
        <td> cp -r</td>
        <td> Copies directories recursively</td>
        <td> cp -r projects/ backup-projects/</td>
    </tr>
    <tr>
        <td> mv</td>
        <td> Moves or renames files/directories</td>
        <td> mv notes.txt /home/user/docs/</td>
    </tr>
    <tr>
        <td> mv</td>
        <td> Rename a file</td>
        <td> mv backup-notes.txt newnotes.txt</td>
    </tr>
    </tbody>
</table>


<br>

### VIEW FILE CONTENTS
<table>
    <thead>
    <tr>
        <th> Command</th>
        <th> Description</th>
        <th> Example</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> cat</td>
        <td> Displays entire file content</td>
        <td> cat notes.txt</td>
    </tr>
    <tr>
        <td> less</td>
        <td> View file one page at a time</td>
        <td> less largefile.txt</td>
    </tr>
    <tr>
        <td> head</td>
        <td> Shows the first 10 lines (default)</td>
        <td> head notes.txt</td>
    </tr>
    <tr>
        <td> tail</td>
        <td> Shows the last 10 lines (default)</td>
        <td> tail notes.txt</td>
    </tr>
    <tr>
        <td> tail -f</td>
        <td> Follow log file in real time</td>
        <td> tail -f /var/log/syslog</td>
    </tr>
    </tbody>
</table>												

<br>

### WILDCARDS AND GLOBBING
<table>
    <thead>
    <tr>
        <th> Wildcard</th>
        <th> Meaning</th>
        <th> Example</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> *</td>
        <td> Matches any number of characters</td>
        <td> ls *.txt → lists all .txt files</td>
    </tr>
    <tr>
        <td> ?</td>
        <td> Matches exactly one character</td>
        <td> ls file?.txt → file1.txt, file2.txt</td>
    </tr>
    <tr>
        <td> [ ]</td>
        <td> Matches one character from a set/range</td>
        <td> ls file[1-3].txt → file1.txt to 3</td>
    </tr>
    </tbody>
</table>


<br>

### LINUX EDITOR
<table>
    <thead>
    <tr>
        <th> Feature</th>
        <th> vi / vim</th>
        <th> nano</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> Interface</td>
        <td> Mode-based (Normal, Insert, etc.)</td>
        <td> Simple and user-friendly</td>
    </tr>
    <tr>
        <td> Learning Curve</td>
        <td> Steep (requires practice)</td>
        <td> Easy for beginners</td>
    </tr>
    <tr>
        <td> Installed by Default</td>
        <td> Yes (on most Linux systems)</td>
        <td> Often pre-installed, else easy to install</td>
    </tr>
    <tr>
        <td> Keyboard Commands</td>
        <td> Complex (:wq, dd, yy, etc.)</td>
        <td> Basic (Ctrl + O, Ctrl + X, etc.)</td>
    </tr>
    <tr>
        <td> Usage</td>
        <td> Preferred for scripting and power users</td>
        <td> Preferred for quick edits</td>
    </tr>
    <tr>
        <td> Navigation</td>
        <td> Arrow keys and commands</td>
        <td> Arrow keys</td>
    </tr>
    <tr>
        <td> Customization</td>
        <td> Highly customizable (.vimrc)</td>
        <td> Limited customization</td>
    </tr>
    </tbody>
</table>												


<br>

### LINUX EDITOR - NANO
<table>
    <thead>
    <tr>
        <th> Command</th>
        <th> Description</th>
        <th> Example</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> nano filename</td>
        <td> Open or create a file</td>
        <td> nano myfile.txt</td>
    </tr>
    <tr>
        <td> Ctrl + O</td>
        <td> Write (save) file</td>
        <td> Press Ctrl + O, then Enter</td>
    </tr>
    <tr>
        <td> Ctrl + X</td>
        <td> Exit nano editor</td>
        <td> Press Ctrl + X</td>
    </tr>
    <tr>
        <td> Ctrl + G</td>
        <td> Help menu</td>
        <td> Lists all commands</td>
    </tr>
    <tr>
        <td> Ctrl + K</td>
        <td> Cut (delete) the current line</td>
        <td> Place cursor on line and press Ctrl + K</td>
    </tr>
    <tr>
        <td> Ctrl + U</td>
        <td> Paste the cut text</td>
        <td> Press after using Ctrl + K</td>
    </tr>
    <tr>
        <td> Ctrl + C</td>
        <td> Show cursor position (line/column)</td>
        <td> Shows line number at bottom</td>
    </tr>
    <tr>
        <td> Ctrl + W</td>
        <td> Search for text</td>
        <td> Ctrl + W, then type keyword</td>
    </tr>
    <tr>
        <td> Ctrl + \</td>
        <td> Replace text</td>
        <td> Ctrl + \, enter old and new text</td>
    </tr>
    <tr>
        <td> Ctrl + _</td>
        <td> Go to a specific line number</td>
        <td> Ctrl + _, then type line number</td>
    </tr>
    <tr>
        <td> Alt + U</td>
        <td> Undo previous action</td>
        <td> Reverts last change</td>
    </tr>
    <tr>
        <td> Alt + E</td>
        <td> Redo (after undo)</td>
        <td> Re-applies last undone change</td>
    </tr>
    </tbody>
</table>												


<br>

### PRIVILEGE TYPES AND FILE PERMISSION
<table>
    <thead>
    <tr>
        <th colspan="3"> Permission Types</th>
    </tr>
    <tr>
        <th> Symbol</th>
        <th> Type</th>
        <th> Description</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> r</td>
        <td> Read</td>
        <td> View file contents or list directory</td>
    </tr>
    <tr>
        <td> w</td>
        <td> Write</td>
        <td> Modify file or create/delete in directory</td>
    </tr>
    <tr>
        <td> x</td>
        <td> Execute</td>
        <td> Run files (like scripts or binaries)</td>
    </tr>
    </tbody>
</table>

<br>

<table>
    <thead>
    <tr>
        <th colspan="3"> Permission Groups</th>
    </tr>
    <tr>
        <th> Symbol</th>
        <th> Group</th>
        <th> Description</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> u</td>
        <td> Owner</td>
        <td> Creator of file; personal access rights</td>
    </tr>
    <tr>
        <td> g</td>
        <td> Group</td>
        <td> Users in the same group as file owner</td>
    </tr>
    <tr>
        <td> o</td>
        <td> Others</td>
        <td> Everyone else on the system</td>
    </tr>
    <tr>
        <td> a</td>
        <td> All</td>
        <td> Applies to all above (u+g+o)</td>
    </tr>
    </tbody>
</table>												


<br>

### PRIVILEGE TYPES AND FILE PERMISSION
<table>
    <thead>
    <tr>
        <th> OCTAL</th>
        <th> DECIMAL</th>
        <th colspan="2"> TYPE OF PRIVILEGES (PERMISSIONS)</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> 000</td>
        <td> 0 (0+0+0)</td>
        <td> No Permission</td>
        <td> - - -</td>
    </tr>
    <tr>
        <td> 001</td>
        <td> 1 (0+0+1)</td>
        <td> Execute</td>
        <td> - - x</td>
    </tr>
    <tr>
        <td> 010</td>
        <td> 2 (0+2+0)</td>
        <td> Write</td>
        <td> - w -</td>
    </tr>
    <tr>
        <td> 011</td>
        <td> 3 (0+2+1)</td>
        <td> Write + Execute</td>
        <td> - w x</td>
    </tr>
    <tr>
        <td> 100</td>
        <td> 4(4+0+0)</td>
        <td> Read</td>
        <td> r - -</td>
    </tr>
    <tr>
        <td> 101</td>
        <td> 5 (4+0+1)</td>
        <td> Read + Execute</td>
        <td> r - x</td>
    </tr>
    <tr>
        <td> 110</td>
        <td> 6 (4+2+0)</td>
        <td> Read + Write</td>
        <td> rw-</td>
    </tr>
    <tr>
        <td> 111</td>
        <td> 7 (4+2+1)</td>
        <td> Read + Write + Execute</td>
        <td> r w x</td>
    </tr>
    </tbody>
</table>															
<table>
    <thead>
    <tr>
        <th> Code</th>
        <th> PRIVILEGES (Description)</th>
        <th> SYNTAX</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> 000</td>
        <td> no permission</td>
        <td> ----------</td>
    </tr>
    <tr>
        <td> 700</td>
        <td> read, write, & execute only for owner</td>
        <td> -rwx------</td>
    </tr>
    <tr>
        <td> 770</td>
        <td> read, write, & execute for owner and group</td>
        <td> -rwxrwx---</td>
    </tr>
    <tr>
        <td> 777</td>
        <td> read, write, & execute for owner, group and others</td>
        <td> -rwxrwxrwx</td>
    </tr>
    <tr>
        <td> 111</td>
        <td> execute</td>
        <td> ---x--x--x</td>
    </tr>
    <tr>
        <td> 222</td>
        <td> write</td>
        <td> --w--w--w-</td>
    </tr>
    <tr>
        <td> 333</td>
        <td> write & execute</td>
        <td> --wx-wx-wx</td>
    </tr>
    <tr>
        <td> 444</td>
        <td> read</td>
        <td> -r--r--r--</td>
    </tr>
    <tr>
        <td> 555</td>
        <td> read & execute</td>
        <td> -r-xr-xr-x</td>
    </tr>
    <tr>
        <td> 666</td>
        <td> read & write</td>
        <td> -rw-rw-rw-</td>
    </tr>
    <tr>
        <td> 740</td>
        <td> owner can read, write, & execute; group can only read; others have no permissions</td>
        <td> -rwxr-----</td>
    </tr>
    </tbody>
</table>												
<table>
    <thead>
    <tr>
        <th> SYNTAX</th>
        <th> Description</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> chown</td>
        <td> Used to change user ownership of a file or directory</td>
    </tr>
    <tr>
        <td> chgrp</td>
        <td> Used to change group ownership</td>
    </tr>
    <tr>
        <td> chmod</td>
        <td> Used to change the permissions on the file, which can be done separately for owner, group and the rest of
            the world (often named as other)
        </td>
    </tr>
    </tbody>
</table>									




<br>

### USER CREATION
<table>
    <thead>
    <tr>
        <th> Command</th>
        <th> Description</th>
        <th> Example</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> adduser</td>
        <td> Adds a new user and prompts for password & details</td>
        <td> sudo adduser user1</td>
    </tr>
    <tr>
        <td> useradd</td>
        <td> Adds user (less interactive than adduser)</td>
        <td> sudo useradd user2</td>
    </tr>
    </tbody>
</table>												




<br>

### GROUP CREATION
<table>
    <thead>
    <tr>
        <th> Command</th>
        <th> Description</th>
        <th> Example</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> groupadd</td>
        <td> Creates a new user group</td>
        <td> sudo groupadd it</td>
    </tr>
    <tr>
        <td> usermod -aG</td>
        <td> Add user to existing group</td>
        <td> sudo usermod -aG it zaheer</td>
    </tr>
    </tbody>
</table>												


<br>

### SETTING PASSWORD
<table>
    <thead>
    <tr>
        <th> Command</th>
        <th> Description</th>
        <th> Example</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> passwd</td>
        <td> Sets or changes password</td>
        <td> sudo passwd alice</td>
    </tr>
    </tbody>
</table>

<br>

### VIEWING USERS AND GROUPS
<table>
    <thead>
    <tr>
        <th> Command</th>
        <th> Description</th>
        <th> Example</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> who</td>
        <td> Shows who is logged in</td>
        <td> who</td>
    </tr>
    <tr>
        <td> id</td>
        <td> Shows current user ID and groups</td>
        <td> id alice</td>
    </tr>
    <tr>
        <td> groups</td>
        <td> Lists group membership</td>
        <td> groups alice</td>
    </tr>
    <tr>
        <td> all users</td>
        <td> List of users</td>
        <td> cat /etc/passwd</td>
    </tr>
    </tbody>
</table>

<br>

### DELETING USERS OR GROUPS
<table>
    <thead>
    <tr>
        <th> Command</th>
        <th> Description</th>
        <th> Example</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> userdel</td>
        <td> Deletes a user</td>
        <td> sudo userdel alice</td>
    </tr>
    <tr>
        <td> groupdel</td>
        <td> Deletes a group</td>
        <td> sudo groupdel admin</td>
    </tr>
    </tbody>
</table>												


<br><br>