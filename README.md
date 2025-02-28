
<h2>                              POSIX Shell Scripting Cheat Sheet</h2>

<table>
    <thead>
        <tr>
            <th>Category</th>
            <th>Syntax / Command</th>
            <th>Description</th>
        </tr>
    </thead>
    <tbody>
        <tr><td>Text Manipulation</td><td><code>echo "Hello, World!"</code></td><td>Prints text to the terminal.</td></tr>
        <tr><td>Text Manipulation</td><td><code>printf "Name: %s\n" "Alice"</code></td><td>Formatted output.</td></tr>
        <tr><td>Arithmetic</td><td><code>expr 5 + 3</code></td><td>Basic arithmetic.</td></tr>
        <tr><td>Variables</td><td><code>VAR="value"</code></td><td>Assigns a value to a variable.</td></tr>
        <tr><td>Loops</td><td><code>for i in {1..5}; do echo $i; done</code></td><td>For loop.</td></tr>
        <tr><td>Control Flow</td><td><code>if [ "$x" -eq 10 ]; then echo "Yes"; fi</code></td><td>If statement.</td></tr>
        <tr><td>Functions</td><td><code>my_func() { echo "Hello"; }</code></td><td>Defines a function.</td></tr>
        <tr><td>File Operations</td><td><code>touch file.txt</code></td><td>Creates an empty file.</td></tr>
        <tr><td>Process Management</td><td><code>ps aux</code></td><td>Lists running processes.</td></tr>
        <tr><td>Redirections</td><td><code>command > file.txt</code></td><td>Redirects output to a file.</td></tr>
        <tr><td>Pipes</td><td><code>command1 | command2</code></td><td>Pipes output of one command to another.</td></tr>
    </tbody>
</table>

<h2>PCRE (Perl-Compatible Regular Expressions) Cheat Sheet</h2>

<table>
    <thead>
        <tr>
            <th>Pattern</th>
            <th>Description</th>
            <th>Example</th>
        </tr>
    </thead>
    <tbody>
        <tr><td><code>.</code></td><td>Matches any single character (except newline).</td><td><code>/a.c/</code> matches "abc", "adc", "a#c"</td></tr>
        <tr><td><code>\d</code></td><td>Matches any digit (0-9).</td><td><code>/\d+/</code> matches "123", "42"</td></tr>
        <tr><td><code>\D</code></td><td>Matches any non-digit.</td><td><code>/\D+/</code> matches "abc", "hello"</td></tr>
        <tr><td><code>\w</code></td><td>Matches any word character (a-z, A-Z, 0-9, _).</td><td><code>/\w+/</code> matches "hello_123"</td></tr>
        <tr><td><code>\W</code></td><td>Matches any non-word character.</td><td><code>/\W+/</code> matches "!!!", "@@@"</td></tr>
        <tr><td><code>\s</code></td><td>Matches any whitespace (space, tab, newline).</td><td><code>/\s+/</code> matches spaces</td></tr>
        <tr><td><code>\S</code></td><td>Matches any non-whitespace character.</td><td><code>/\S+/</code> matches "word"</td></tr>
        <tr><td><code>^</code></td><td>Matches the start of a line.</td><td><code>/^abc/</code> matches "abc" at start</td></tr>
        <tr><td><code>$</code></td><td>Matches the end of a line.</td><td><code>/abc$/</code> matches "abc" at end</td></tr>
        <tr><td><code>[abc]</code></td><td>Matches any character inside brackets.</td><td><code>/[aeiou]/</code> matches vowels</td></tr>
        <tr><td><code>[^abc]</code></td><td>Matches any character NOT in brackets.</td><td><code>/[^0-9]/</code> matches non-digits</td></tr>
        <tr><td><code>(...)</code></td><td>Capturing group.</td><td><code>/(hello)/</code> captures "hello"</td></tr>
        <tr><td><code>|</code></td><td>Logical OR.</td><td><code>/cat|dog/</code> matches "cat" or "dog"</td></tr>
        <tr><td><code>*</code></td><td>Matches 0 or more occurrences.</td><td><code>/a*/</code> matches "", "a", "aaa"</td></tr>
        <tr><td><code>+</code></td><td>Matches 1 or more occurrences.</td><td><code>/a+/</code> matches "a", "aaa"</td></tr>
        <tr><td><code>?</code></td><td>Matches 0 or 1 occurrences.</td><td><code>/a?/</code> matches "", "a"</td></tr>
        <tr><td><code>{n}</code></td><td>Matches exactly n times.</td><td><code>/a{3}/</code> matches "aaa"</td></tr>
        <tr><td><code>{n,}</code></td><td>Matches n or more times.</td><td><code>/a{2,}/</code> matches "aa", "aaa"</td></tr>
        <tr><td><code>{n,m}</code></td><td>Matches between n and m times.</td><td><code>/a{2,4}/</code> matches "aa", "aaa", "aaaa"</td></tr>
    </tbody>
</table>

</body>
</html>
