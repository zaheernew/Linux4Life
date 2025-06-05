<br><br>

[< Linux4Life](https://github.com/zaheernew/Linux4Life/blob/main/Linux4Life.md)

# Module 9

<br>

## BASH SCRIPTING - SHELL

\
A shell script is a plain text file containing a sequence of commands for a Unix-based shell (like Bash) to execute.\
Helps automate repetitive tasks (e.g., backups, system checks).\
Script files typically have .sh extension but it's not mandatory.\
\
Example : (type in the terminal)\
echo "Welcome to Linux scripting"\
\
\
\
SHEBANG (#!/bin/bash)\
The shebang (#!) at the beginning of a script tells the system which interpreter to use.\
#!/bin/bash → Uses Bash shell to execute the script.\
\
Example : (type in the terminal)\
#!/bin/bash\
echo "Script started"\
<br>
<br>
<br>
<h3>Variables and Conditions</h3>
#!/bin/bash <br>
name="Linux" <br>
if [ "$name" == "Linux" ]; then <br> 
  echo "Welcome, $name user!" <br>
fi <br>
<br>
<br>
<br>
<h3>Loops and Functions</h3>
Loops (for, while) help repeat tasks.\
Functions group code into reusable blocks.\
\
Example : (type in the terminal)\
#!/bin/bash\ <br>
greet() {\ <br>
echo "Hello, $1!" <br>
} <br>
for user in Zaheer Saman Siva; do <br>
greet $user <br>
done <br>
<br>
<br>
<br>
<h3>Make Simple Script</h3>
To run a script directly, you must make it executable.\
\
Example :\
nano hello.sh\
Add the wording (type in the terminal)\
<br>
#!/bin/bash<br>
echo "Hello, Linux !”<br>
date<br>
<br>
Now save and change it to the executable.\
chmod +x hello.sh\
Now run ./hello.sh\
<br>
<br>
<br>
<h3>Make Script Executable</h3>
To run a script directly, you must make it executable.\
chmod +x hello.sh\
\
Use the same file – last example :\
(type in the terminal) – sudo nano hello.sh\
#!/bin/bash\
greet() {\
echo "Hello, \$1!"\
}\
for user in Zaheer Saman Siva; do\
greet \$user\
done

<br><br>
