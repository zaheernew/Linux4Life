<br><br>

[< Linux4Life](https://github.com/zaheernew/Linux4Life/blob/main/Linux4Life.md)

# Module 6

<br>

## PROCESS AND SERVICE MANAGEMENT

<br>


### Viewing Processes
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
        <td> ps</td>
        <td> Lists currently running processes (snapshot).</td>
        <td> ps aux</td>
    </tr>
    <tr>
        <td> top</td>
        <td> Real-time view of running processes.</td>
        <td> top</td>
    </tr>
    <tr>
        <td> htop</td>
        <td> Interactive, color-enhanced process viewer.</td>
        <td> htop (may need install)</td>
    </tr>
    <tr>
        <td> cpuinfo</td>
        <td> Get CPU information</td>
        <td> cat /proc/cpuinfo</td>
    </tr>
    </tbody>
</table>												



<br>

### Killing or Stopping Processes
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
        <td> kill PID</td>
        <td> Terminates a process by its Process ID (PID).</td>
        <td> kill 1234</td>
    </tr>
    <tr>
        <td> killall name</td>
        <td> Kills all processes with a given name.</td>
        <td> killall firefox</td>
    </tr>
    </tbody>
</table>												




<br>

### Background Process Management
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
        <td> &</td>
        <td> Runs a command in the background.</td>
        <td> ping google.com &</td>
    </tr>
    <tr>
        <td> jobs</td>
        <td> Lists current background jobs.</td>
        <td> jobs</td>
    </tr>
    <tr>
        <td> fg</td>
        <td> Brings a background job to the foreground.</td>
        <td> fg %1</td>
    </tr>
    <tr>
        <td> bg</td>
        <td> Resumes a stopped job in the background.</td>
        <td> bg %1</td>
    </tr>
    </tbody>
</table>												




<br>

### Managing Services
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
        <td> systemctl status</td>
        <td> Shows service status (active/inactive/failed).</td>
        <td> systemctl status apache2</td>
    </tr>
    <tr>
        <td> systemctl start</td>
        <td> Starts a service.</td>
        <td> sudo systemctl start ssh</td>
    </tr>
    <tr>
        <td> systemctl stop</td>
        <td> Stops a service.</td>
        <td> sudo systemctl stop apache2</td>
    </tr>
    <tr>
        <td> service name status</td>
        <td> Older command to check service status.</td>
        <td> service apache2 status</td>
    </tr>
    </tbody>
</table>												



<br>

### Viewing Logs
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
        <td> journalctl</td>
        <td> Views systemd logs.</td>
        <td> journalctl -xe</td>
    </tr>
    <tr>
        <td> /var/log</td>
        <td> Default location for traditional log files.</td>
        <td> cat /var/log/syslog</td>
    </tr>
    </tbody>
</table>												

<br><br>
