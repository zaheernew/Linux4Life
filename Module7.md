<br><br>

[< Linux4Life](https://github.com/zaheernew/Linux4Life/blob/main/Linux4Life.md)

# Module 7

<br>

## NETWORKING BASICS
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
        <td> ip a</td>
        <td> Shows all IP addresses and network interfaces.</td>
        <td> ip a</td>
    </tr>
    <tr>
        <td> ifconfig</td>
        <td> Displays IP info (older tool; may need net-tools).</td>
        <td> ifconfig</td>
    </tr>
    <tr>
        <td> hostname</td>
        <td> Displays or sets the system hostname.</td>
        <td> hostname</td>
    </tr>
    <tr>
        <td> nslookup
            <domain>
        </td>
        <td> Performs DNS lookup for domain name resolution.</td>
        <td> nslookup ou.ac.lk</td>
    </tr>
    <tr>
        <td> dig
            <domain>
        </td>
        <td> Detailed DNS query tool for domain/IP information.</td>
        <td> dig ou.ac.lk</td>
    </tr>
    </tbody>
</table>												


<br>


### Testing Connectivity
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
        <td> ping
            <host>
        </td>
        <td> Tests reachability by sending ICMP echo requests.</td>
        <td> ping google.com</td>
    </tr>
    <tr>
        <td> traceroute
            <host>
        </td>
        <td> Traces route to destination, showing intermediate hops.</td>
        <td> traceroute 8.8.8.8</td>
    </tr>
    <tr>
        <td> ss</td>
        <td> Displays socket statistics (modern alternative).</td>
        <td> ss -tuln</td>
    </tr>
    <tr>
        <td> netstat -a | more</td>
        <td> To show both listening and non-listening sockets.</td>
        <td> netstat -a | more <br> netstat -anp </td>
    </tr>
    <tr>
        <td> netstat -at</td>
        <td> To list all tcp ports.</td>
        <td> netstat -at</td>
    </tr>
    <tr>
        <td> netstat -au</td>
        <td> To list all udp ports.</td>
        <td> netstat -au</td>
    </tr>
    <tr>
        <td> netstat -l</td>
        <td> To list only the listening ports.</td>
        <td> netstat –l or ss -lntu</td>
    </tr>
    <tr>
        <td> netstat -lt</td>
        <td> To list only the listening tcp ports.</td>
        <td> netstat -lt</td>
    </tr>
    <tr>
        <td> netstat -lu</td>
        <td> To list only the listening udp ports.</td>
        <td> netstat -lu</td>
    </tr>
    </tbody>
</table>												


<br>

### Network Configuration Files and Tools
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
        <td> /etc/network/interfaces</td>
        <td> File to configure IP settings (older Debian systems).</td>
        <td> nano /etc/network/interfaces/00-installer-config.yaml</td>
    </tr>
    </tbody>
</table>												



<br><br>
