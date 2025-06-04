<br><br>

[< Linux4Life](https://github.com/zaheernew/Linux4Life/blob/main/Linux4Life.md)

# Module 1

## Linux symbols

<table>
  <thead>
    <tr>
      <th>Symbol</th>
      <th>Name</th>
      <th>Meaning / Use</th>
      <th>Example</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>~</td><td>Tilde</td><td>Home directory of the current user (= go to home)</td><td>cd ~</td></tr>
    <tr><td>/</td><td>Slash</td><td>Directory separator / root</td><td>/etc/passwd</td></tr>
    <tr><td>.</td><td>Dot</td><td>Current directory</td><td>./script.sh</td></tr>
    <tr><td>..</td><td>Double dot</td><td>Parent directory (= move up)</td><td>cd ..</td></tr>
    <tr><td>-</td><td>Dash</td><td>Option/flag for a command</td><td>ls -l</td></tr>
    <tr><td>*</td><td>Asterisk</td><td>Wildcard for any characters</td><td>ls *.txt</td></tr>
    <tr><td>|</td><td>Pipe</td><td>Send output of one command to another</td><td>`</td></tr>
    <tr><td>></td><td>Redirect</td><td>Redirect output to a file (overwrite)</td><td>echo hi > file.txt</td></tr>
    <tr><td>>></td><td>Append Redirect</td><td>Append output to a file</td><td>echo bye >> file.txt</td></tr>
    <tr><td><</td><td>Input Redirect</td><td>Take input from a file</td><td>sort &lt; file.txt</td></tr>
    <tr><td>&</td><td>Background</td><td>Run a command in the background</td><td>firefox &</td></tr>
    <tr><td>&&</td><td>AND operator</td><td>Run second command if first succeeds</td><td>mkdir test && cd test</td></tr>
    <tr><td>||</td><td>OR operator</td><td>Run second command if first fails</td><td>(example not provided)</td></tr>
    <tr><td>#</td><td>Hash / Pound</td><td>Comment in shell scripts or config files</td><td># This is a comment</td></tr>
    <tr><td>\</td><td>Backslash</td><td>Escape special characters</td><td>echo \\"Hello\\"</td></tr>
  </tbody>
</table>
<br><br>
