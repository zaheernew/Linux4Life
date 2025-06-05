<br><br>

[< Linux4Life](https://github.com/zaheernew/Linux4Life/blob/main/Linux4Life.md)

# Module 10

<br>

## SECURITY, UPDATES, AND TROUBLESHOOTING

<br>
<h3>Security</h3>
<h3>UFW - Uncomplicated Firewall Simplifies iptables rule management</h3>
<table>
    <thead>
    <tr>
        <th> Function</th>
        <th> Descriptions</th>
        <th> Command</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> Activates the firewall</td>
        <td> Enables protection</td>
        <td> sudo ufw enable</td>
    </tr>
    <tr>
        <td> Deactivates the firewall</td>
        <td> Turns off UFW</td>
        <td> sudo ufw disable</td>
    </tr>
    <tr>
        <td> View current status and rules</td>
        <td> Shows active rules</td>
        <td> sudo ufw status</td>
    </tr>
    <tr>
        <td> Shows detailed output</td>
        <td> Verbose rule list</td>
        <td> sudo ufw status verbose</td>
    </tr>
    <tr>
        <td> Reloads rules (use after config changes)</td>
        <td> Apply rule changes</td>
        <td> sudo ufw reload</td>
    </tr>
    <tr>
        <td> Allow SSH</td>
        <td> Allows incoming SSH connections</td>
        <td> sudo ufw allow ssh or sudo ufw allow 22</td>
    </tr>
    </tbody>
</table>	

<br>

### Updating System Packages
<table>
    <thead>
    <tr>
        <th> Function</th>
        <th> Descriptions</th>
        <th> Command</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> To update</td>
        <td> Refreshes package list from repositories</td>
        <td> sudo apt update</td>
    </tr>
    <tr>
        <td> To upgrade</td>
        <td> Installs available updates for installed packages</td>
        <td> sudo apt upgrade</td>
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
        <td> cat</td>
        <td> Outputs entire file contents (only support – rsyslog)</td>
        <td> cat /var/log/syslog</td>
    </tr>
    <tr>
        <td> head</td>
        <td> Shows first 10 lines</td>
        <td> head /var/log/syslog</td>
    </tr>
    <tr>
        <td> tail</td>
        <td> Shows last 10 lines</td>
        <td> tail /var/log/syslog</td>
    </tr>
    <tr>
        <td> tail -f</td>
        <td> Live updates as log grows</td>
        <td> tail -f /var/log/syslog</td>
    </tr>
    <tr>
        <td> less</td>
        <td> Scrollable view (forward/backward)</td>
        <td> less /var/log/syslog</td>
    </tr>
    <tr>
        <td> grep</td>
        <td> Search specific keywords</td>
        <td> grep "error" /var/log/syslog</td>
    </tr>
    <tr>
        <td> journalctl</td>
        <td> View logs with systemd</td>
        <td> journalctl -xe</td>
    </tr>
    <tr>
        <td> journalctl</td>
        <td> kernel/system logs</td>
        <td> journalctl -k</td>
    </tr>
    <tr>
        <td> journalctl</td>
        <td> check logs from previous boots</td>
        <td> journalctl --list-boots</td>
    </tr>
    <tr>
        <td> dmesg</td>
        <td> Boot/kernel logs</td>
        <td> dmesg</td>
    </tr>
    </tbody>
</table>												


<br>

### Managing Services

<table>
    <thead>
    <tr>
        <th> Action</th>
        <th> Command (systemd)</th>
        <th> Purpose</th>
        <th> Example</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> Enable</td>
        <td> sudo systemctl enable service-name</td>
        <td> Enables the service to start at boot time</td>
        <td> sudo systemctl enable apache2</td>
    </tr>
    <tr>
        <td> Start</td>
        <td> sudo systemctl start service-name</td>
        <td> Starts the service immediately</td>
        <td> sudo systemctl start apache2</td>
    </tr>
    <tr>
        <td> Restart</td>
        <td> sudo systemctl restart service-name</td>
        <td> Restarts the service (use after config changes)</td>
        <td> sudo systemctl restart apache2</td>
    </tr>
    <tr>
        <td> Stop</td>
        <td> sudo systemctl stop service-name</td>
        <td> Stops the service</td>
        <td> sudo systemctl stop apache2</td>
    </tr>
    <tr>
        <td> Status</td>
        <td> sudo systemctl status service-name</td>
        <td> Displays current status (running, inactive, failed, etc.)</td>
        <td> sudo systemctl status apache2</td>
    </tr>
    </tbody>
</table>															



<br><br>
