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
