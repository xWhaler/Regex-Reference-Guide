
<h2>                             Shell Scripting Cheat Sheet</h2>

<h5>See python-specific-regex.md for python-specific identifiers.</h5>

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

<h1> Common Regex identifiers </h1>
<h3>Perl-compatible Regular Expressions (PCRE)</h3>

<table>
    <thead>
        <tr>
            <th>Regex</th>
            <th>Description</th>
            <th>Example</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>.</td>
            <td>Matches any single character except a newline (\n)</td>
            <td>h.t matches hat, hit, but not h/t.</td>
        </tr>
        <tr>
            <td>^</td>
            <td>Anchors to the start of a string or line</td>
            <td>^Hello matches "Hello" at the beginning of a string.</td>
        </tr>
        <tr>
            <td>$</td>
            <td>Anchors to the end of a string or line</td>
            <td>world$ matches "world" at the end of a string.</td>
        </tr>
        <tr>
            <td>\</td>
            <td>Escape character for special symbols</td>
            <td>\. matches a literal .</td>
        </tr>
        <tr>
            <td>[]</td>
            <td>Character class, matches any single character within</td>
            <td>[aeiou] matches any vowel.</td>
        </tr>
        <tr>
            <td>[^]</td>
            <td>Negated character class, matches any single character not within</td>
            <td>[^aeiou] matches any non-vowel.</td>
        </tr>
        <tr>
            <td>|</td>
            <td>Alternation (logical OR)</td>
            <td></td>
        </tr>
        <tr>
            <td>()</td>
            <td>Capturing group; groups patterns and captures the match for later reference</td>
            <td>(ab)+ matches "ab", "abab", etc.</td>
        </tr>
        <tr>
            <td>(?: )</td>
            <td>Non-capturing group; groups patterns without capturing them</td>
            <td>(?:ab)+ matches "abab" but doesn’t capture it.</td>
        </tr>
        <tr>
            <td>{}</td>
            <td>Quantifier specifying exact or range repetitions</td>
            <td>a{3} matches "aaa". a{2,4} matches "aa", "aaa", or "aaaa".</td>
        </tr>
        <tr>
            <td>*</td>
            <td>Matches 0 or more of the preceding character or group</td>
            <td>a* matches "", "a", "aa", etc.</td>
        </tr>
        <tr>
            <td>+</td>
            <td>Matches 1 or more of the preceding character or group</td>
            <td>a+ matches "a", "aa", etc., but not "".</td>
        </tr>
        <tr>
            <td>?</td>
            <td>Matches 0 or 1 of the preceding character or group; makes quantifiers lazy when placed after</td>
            <td>a? matches "", or "a". a*? matches as few "a"s as possible.</td>
        </tr>
        <tr>
            <td>/</td>
            <td>Delimiter for regex in some languages like JavaScript or Perl</td>
            <td>/hello/ matches "hello".</td>
        </tr>
        <tr>
            <td>\d</td>
            <td>Matches any digit (0-9)</td>
            <td>\d{2} matches "12".</td>
        </tr>
        <tr>
            <td>\D</td>
            <td>Matches any non-digit</td>
            <td>\D matches "a", but not "2".</td>
        </tr>
        <tr>
            <td>\w</td>
            <td>Matches any word character (alphanumeric + underscore)</td>
            <td>\w+ matches "word123".</td>
        </tr>
        <tr>
            <td>\W</td>
            <td>Matches any non-word character</td>
            <td>\W matches "@", but not "a".</td>
        </tr>
        <tr>
            <td>\s</td>
            <td>Matches any whitespace character (spaces, tabs, newlines)</td>
            <td>\s+ matches spaces between words.</td>
        </tr>
        <tr>
            <td>\S</td>
            <td>Matches any non-whitespace character</td>
            <td>\S+ matches "word123", but not " ".</td>
        </tr>
        <tr>
            <td>\b</td>
            <td>Matches a word boundary</td>
            <td>\bword\b matches "word", but not "sword".</td>
        </tr>
        <tr>
            <td>\B</td>
            <td>Matches a position that is not a word boundary</td>
            <td>\Bword matches "sword", but not " word".</td>
        </tr>
    </tbody>

</body>
</html>
