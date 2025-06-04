<br><br>

[< Linux4Life](https://github.com/zaheernew/Linux4Life/blob/main/Linux4Life.md)

# Module 2

<br>

## Basic Commands

<br>

### File & Directory Navigation
<table>
  <tr>
    <th>Command</th>
    <th>Description</th>
    <th>Example</th>
  </tr>
  <tr>
    <td>pwd</td>
    <td>Show current working directory</td>
    <td>pwd</td>
  </tr>
  <tr>
    <td>ls</td>
    <td>List files and directories</td>
    <td>ls</td>
  </tr>
  <tr>
    <td>ls -l</td>
    <td>Long listing format</td>
    <td>ls -l</td>
  </tr>
  <tr>
    <td>ls -a</td>
    <td>Show hidden files</td>
    <td>ls -a</td>
  </tr>
  <tr>
    <td>ls -lh</td>
    <td>Human-readable long list</td>
    <td>ls -lh</td>
  </tr>
  <tr>
    <td>cd</td>
    <td>Change directory</td>
    <td>cd /home/user</td>
  </tr>
  <tr>
    <td>cd ..</td>
    <td>Move to parent directory</td>
    <td>cd ..</td>
  </tr>
  <tr>
    <td>cd ~</td>
    <td>Move to home directory</td>
    <td>cd ~</td>
  </tr>
  <tr>
    <td>mkdir</td>
    <td>Create new directory</td>
    <td>mkdir test_dir</td>
  </tr>
  <tr>
    <td>rmdir</td>
    <td>Remove empty directory</td>
    <td>rmdir test_dir</td>
  </tr>
  <tr>
    <td>rm</td>
    <td>Remove a file</td>
    <td>rm test.txt</td>
  </tr>
  <tr>
    <td>rm -r</td>
    <td>Remove a directory and contents</td>
    <td>rm -r folder/</td>
  </tr>
</table>

<br>

### File Operations and Viewing
<table>
  <tr>
    <th>Command</th>
    <th>Description</th>
    <th>Example</th>
  </tr>
  <tr>
    <td>touch</td>
    <td>Create a new empty file</td>
    <td>touch index.html</td>
  </tr>
  <tr>
    <td>cp</td>
    <td>Copy a file</td>
    <td>cp file.txt backup/</td>
  </tr>
  <tr>
    <td>cp -r</td>
    <td>Copy a folder</td>
    <td>cp -r folder1 folder2</td>
  </tr>
  <tr>
    <td>mv</td>
    <td>Move or rename file</td>
    <td>mv a.txt b.txt</td>
  </tr>
  <tr>
    <td>cat</td>
    <td>Show file content</td>
    <td>cat info.txt</td>
  </tr>
  <tr>
    <td>cat file1 file2</td>
    <td>Combine and show files</td>
    <td>cat part1.txt part2.txt</td>
  </tr>
  <tr>
    <td>echo</td>
    <td>Display text</td>
    <td>echo "Linux is cool"</td>
  </tr>
  <tr>
    <td>man</td>
    <td>Open command manual</td>
    <td>man ls</td>
  </tr>
  <tr>
    <td>command --help</td>
    <td>Show help for a command</td>
    <td>ls --help</td>
  </tr>
  <tr>
    <td>clear</td>
    <td>Clear terminal screen</td>
    <td>clear</td>
  </tr>
</table>

<br>

### System, Process & Package
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
        <td> history</td>
        <td> Show previous commands</td>
        <td> history</td>
    </tr>
    <tr>
        <td> uname -a</td>
        <td> Show system information</td>
        <td> uname -a</td>
    </tr>
    <tr>
        <td> whoami</td>
        <td> Show logged-in username</td>
        <td> whoami</td>
    </tr>
    <tr>
        <td> df -h</td>
        <td> Show disk space in human-readable form</td>
        <td> df -h</td>
    </tr>
    <tr>
        <td> top</td>
        <td> View running processes</td>
        <td> top</td>
    </tr>
    <tr>
        <td> kill
            <PID>
        </td>
        <td> Kill a process by PID</td>
        <td> kill 1234</td>
    </tr>
    <tr>
        <td> sudo</td>
        <td> Run command as superuser</td>
        <td> sudo apt update</td>
    </tr>
    <tr>
        <td> apt update</td>
        <td> Update package lists</td>
        <td> sudo apt update</td>
    </tr>
    <tr>
        <td> apt install</td>
        <td> Install a package</td>
        <td> sudo apt install curl</td>
    </tr>
    <tr>
        <td> exit</td>
        <td> Exit terminal</td>
        <td> exit</td>
    </tr>
    </tbody>
</table>


<br>

### Host name changing
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
        <td> hostnamectl</td>
        <td> Check the current hostname</td>
        <td> hostnamectl</td>
    </tr>
    <tr>
        <td> sudo hostnamectl set-hostname your-new-hostname</td>
        <td> Set a new hostname</td>
        <td> sudo hostnamectl set-hostname web-server</td>
    </tr>
    <tr>
        <td> sudo nano /etc/hosts</td>
        <td> Edit /etc/hosts <br> 127.0.1.1 your-new-hostname</td>
        <td> sudo nano /etc/hosts <br> 127.0.1.1 web-server</td>
    </tr>
    <tr>
        <td> exec bash</td>
        <td> To apply</td>
        <td> exec bash</td>
    </tr>
    <tr>
        <td> hostnamectl</td>
        <td> To verify</td>
        <td> hostnamectl</td>
    </tr>
    <tr>
        <td> sudo timedatectl set-timezone Asia/Kolkata</td>
        <td> To set date & time</td>
        <td> sudo timedatectl set-timezone Asia/Kolkata</td>
    </tr>
    </tbody>
</table>												



<br><br>
