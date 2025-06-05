<br><br>

[< Linux4Life](https://github.com/zaheernew/Linux4Life/blob/main/Linux4Life.md)

# Module 8

<br>

## DISK MANAGEMENT

<br>


### Viewing Disk Usage
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
        <td> df -h</td>
        <td> Displays disk space usage in a human-readable format</td>
        <td> df -h</td>
    </tr>
    <tr>
        <td> du -sh</td>
        <td> Shows size of a directory or file</td>
        <td> du -sh /home</td>
    </tr>
    <tr>
        <td> lsblk</td>
        <td> Lists available disks and partitions</td>
        <td> lsblk</td>
    </tr>
    </tbody>
</table>						


<br>

### DISK MANAGEMENT - SWAP
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
        <td> sudo swapon --show</td>
        <td> View Swap Usage</td>
        <td> mount /dev/sdb1 /mnt/usb</td>
    </tr>
    <tr>
        <td> sudo free -h</td>
        <td> view swap space status</td>
        <td> umount /mnt/usb</td>
    </tr>
    </tbody>
</table>												



<br>

### DISK MANAGEMENT - SWAP
<table>
    <thead>
    <tr>
        <th> Field</th>
        <th> Description</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> NAME</td>
        <td> The swap device or file name. Here, /swap.img indicates a swap file.</td>
    </tr>
    <tr>
        <td> TYPE</td>
        <td> Indicates whether it's a file-based or partition-based swap. (file in this case)</td>
    </tr>
    <tr>
        <td> SIZE</td>
        <td> Total swap size (4 GB in this example).</td>
    </tr>
    <tr>
        <td> USED</td>
        <td> Currently used swap space (2.5 MB used—very minimal).</td>
    </tr>
    <tr>
        <td> PRIO</td>
        <td> Swap priority (-2 is the default for swap files; lower means lower priority).</td>
    </tr>
    </tbody>
</table>											





<br>

### DISK MANAGEMENT - SWAP
<table>
    <thead>
    <tr>
        <th> Field</th>
        <th> Description</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td> total</td>
        <td> Total installed memory (RAM = 7.8 GiB, Swap = 4.0 GiB)</td>
    </tr>
    <tr>
        <td> used</td>
        <td> Actual used memory (RAM used = 3.2 GiB, Swap used = 2.0 MiB)</td>
    </tr>
    <tr>
        <td> free</td>
        <td> Completely unused memory (RAM = 907 MiB, Swap = 4.0 GiB free)</td>
    </tr>
    <tr>
        <td> shared</td>
        <td> Memory used by tmpfs (shared between processes, e.g., for /dev/shm)</td>
    </tr>
    <tr>
        <td> buff/cache</td>
        <td> Memory used for buffers and cache (can be reused by apps if needed)</td>
    </tr>
    <tr>
        <td> available</td>
        <td> Estimated memory available for starting new apps without using swap</td>
    </tr>
</table>											



<br><br>
