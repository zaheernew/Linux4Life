<br><br>

[< Linux4Life](https://github.com/zaheernew/Linux4Life/blob/main/Linux4Life.md)

# Module 4

<br>

## User Management

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
