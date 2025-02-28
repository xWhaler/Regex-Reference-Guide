<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>POSIX Shell Scripting Cheat Sheet</title>
    
</head>
<body>

<h2>POSIX Shell Scripting Cheat Sheet</h2>

<table>
    <thead>
        <tr>
            <th>Category</th>
            <th>Syntax / Command</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Text Manipulation</td>
            <td>echo "Hello, World!"</td>
            <td>Prints text to the terminal.</td>
        </tr>
        <tr>
            <td>Text Manipulation</td>
            <td>printf "Name: %s\n" "Alice"</td>
            <td>Formatted output.</td>
        </tr>
        <tr>
            <td>Text Manipulation</td>
            <td>cat file.txt</td>
            <td>Displays the contents of a file.</td>
        </tr>
        <tr>
            <td>Arithmetic</td>
            <td>expr 5 + 3</td>
            <td>Basic arithmetic.</td>
        </tr>
        <tr>
            <td>Arithmetic</td>
            <td>$((5 + 3))</td>
            <td>Arithmetic expansion.</td>
        </tr>
        <tr>
            <td>Variables</td>
            <td>VAR="value"</td>
            <td>Assigns a value to a variable.</td>
        </tr>
        <tr>
            <td>Variables</td>
            <td>echo $VAR</td>
            <td>Prints the variable's value.</td>
        </tr>
        <tr>
            <td>Conditional Expressions</td>
            <td>[ "$x" -eq "$y" ]</td>
            <td>Integer equality check.</td>
        </tr>
        <tr>
            <td>Conditional Expressions</td>
            <td>[ -f file.txt ]</td>
            <td>True if file.txt exists.</td>
        </tr>
        <tr>
            <td>Loops</td>
            <td>for i in {1..5}; do echo $i; done</td>
            <td>For loop.</td>
        </tr>
        <tr>
            <td>Loops</td>
            <td>while [ $x -lt 5 ]; do echo $x; x=$((x+1)); done</td>
            <td>While loop.</td>
        </tr>
        <tr>
            <td>Control Flow</td>
            <td>if [ "$x" -eq 10 ]; then echo "Yes"; fi</td>
            <td>If statement.</td>
        </tr>
        <tr>
            <td>Control Flow</td>
            <td>case $VAR in pattern1) command;; pattern2) command;; esac</td>
            <td>Case statement.</td>
        </tr>
        <tr>
            <td>Functions</td>
            <td>my_func() { echo "Hello"; }</td>
            <td>Defines a function.</td>
        </tr>
        <tr>
            <td>Functions</td>
            <td>my_func</td>
            <td>Calls a function.</td>
        </tr>
        <tr>
            <td>File Operations</td>
            <td>touch file.txt</td>
            <td>Creates an empty file.</td>
        </tr>
        <tr>
            <td>File Operations</td>
            <td>rm file.txt</td>
            <td>Deletes a file.</td>
        </tr>
        <tr>
            <td>Process Management</td>
            <td>ps aux</td>
            <td>Lists running processes.</td>
        </tr>
        <tr>
            <td>Process Management</td>
            <td>kill PID</td>
            <td>Kills a process with a given PID.</td>
        </tr>
        <tr>
            <td>Redirections</td>
            <td>command > file.txt</td>
            <td>Redirects output to a file.</td>
        </tr>
        <tr>
            <td>Redirections</td>
            <td>command < input.txt</td>
            <td>Reads input from a file.</td>
        </tr>
        <tr>
            <td>Pipes</td>
            <td>command1 | command2</td>
            <td>Pipes output of one command to another.</td>
        </tr>
        <tr>
            <td>Pipes</td>
            <td>ls | grep "file"</td>
            <td>Filters `ls` output with `grep`.</td>
        </tr>
    </tbody>
</table>

</body>
</html>
