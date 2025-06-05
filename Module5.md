<br><br>

[< Linux4Life](https://github.com/zaheernew/Linux4Life/blob/main/Linux4Life.md)

# Module 5

<br>

## PACKAGE MANAGEMENT

<br>


### PACKAGE MANAGEMENT: MANAGING
<table>
    <thead>
    <tr>
        <th> Task</th>
        <th> Command</th>
        <th> Purpose</th>
        <th> Example</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> Update System</td>
        <td> sudo apt update</td>
        <td> Refreshes package list.</td>
        <td> sudo apt update</td>
    </tr>
    <tr>
        <td> Upgrade System</td>
        <td> sudo apt upgrade</td>
        <td> Installs latest versions.</td>
        <td> sudo apt upgrade</td>
    </tr>
    <tr>
        <td> Install Software</td>
        <td> sudo apt install package-name</td>
        <td> Installs the specified software with dependencies.</td>
        <td> sudo apt install nano</td>
    </tr>
    <tr>
        <td> Remove Software</td>
        <td> sudo apt remove package-name</td>
        <td> Deletes software only.</td>
        <td> sudo apt remove nano</td>
    </tr>
    <tr>
        <td> Remove Software</td>
        <td> sudo apt purge package-name</td>
        <td> Deletes software + config files.</td>
        <td> sudo apt purge nano</td>
    </tr>
    <tr>
        <td> Package status</td>
        <td> dpkg -s example-package</td>
        <td> Check package status.</td>
        <td> sudo apt dpkg –s nano</td>
    </tr>
    <tr>
        <td> Installed packages</td>
        <td> apt list --installed</td>
        <td> To list all installed packages</td>
        <td> sudo apt list --installed</td>
    </tr>
    <tr>
        <td> Upgradeable packages</td>
        <td> sudo apt list --upgradeable</td>
        <td> To a list of all upgradeable packages</td>
        <td> sudo apt list --upgradeable</td>
    </tr>
    </tbody>
</table>															




<br>

### PACKAGE MANAGEMENT: ESSENTIAL CLI’s
<table>
    <thead>
    <tr>
        <th> Name of Package</th>
        <th> Command</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> Nano – Terminal text editor</td>
        <td> sudo apt install nano</td>
    </tr>
    <tr>
        <td> Curl – Data transfer utility</td>
        <td> sudo apt install curl</td>
    </tr>
    <tr>
        <td> Wget – Download files</td>
        <td> sudo apt install wget</td>
    </tr>
    <tr>
        <td> Net-tools – ifconfig, netstat</td>
        <td> sudo apt install net-tools</td>
    </tr>
    <tr>
        <td> IP Utils (ping) – Ping tool</td>
        <td> sudo apt install iputils-ping</td>
    </tr>
    <tr>
        <td> LSB Release – Distro info tool</td>
        <td> sudo apt install lsb-release</td>
    </tr>
    <tr>
        <td> UFW – Uncomplicated Firewall</td>
        <td> sudo apt install ufw</td>
    </tr>
    <tr>
        <td> Unzip – Extract ZIP archives</td>
        <td> sudo apt install unzip</td>
    </tr>
    <tr>
        <td> Zip – Create ZIP archives</td>
        <td> sudo apt install zip</td>
    </tr>
    <tr>
        <td> Htop – Interactive process viewer</td>
        <td> sudo apt install htop</td>
    </tr>
    <tr>
        <td> Apache2 – Web server</td>
        <td> sudo apt install apache2</td>
    </tr>
    <tr>
        <td> Sudo – Superuser command</td>
        <td> sudo apt install sudo</td>
    </tr>
    <tr>
        <td> Enable Universe Repository</td>
        <td> sudo add-apt-repository universe -y</td>
    </tr>
    </tbody>
</table>									



<br><br>
