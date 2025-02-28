# Python Regular Expressions (Regex) 


<h4>❗ Regex is extremely helpful when you're tasked with manipulating data structures that contain numerous data types.</h4>

<h3> ⏲️ Short History of Regex </h3>
<p>The concept of regular expressions began in the 1950s, when the American mathematician Stephen Cole Kleene formalized the concept of a regular language. 
  They came into common use with Unix text-processing utilities.
  Different syntaxes for writing regular expressions have existed since the 1980s, one being the POSIX standard and another, widely used, being the Perl syntax. </p>


  <p>Similar identifiers are found in those below:
    <li>
       Perl Compatible regular expression (PCRE)
    </li>
    <li>
       POSIX standard
    </li>
    <li>
      Bash scripting language 
    </li>
  </p>
  <h5>Many of these will work across langauges with minor variations in syntax. </h5>


## Example Usage

```python
import re

pattern = re.compile(r'\d+')
match = pattern.search("Order number: 12345")
print(match.group())  # Output: 12345
```

## Metacharacters

| Symbol | Description |
|--------|-------------|
| `.` | Matches any character except newline |
| `^` | Matches start of string |
| `$` | Matches end of string |
| `*` | Matches 0 or more repetitions |
| `+` | Matches 1 or more repetitions |
| `?` | Matches 0 or 1 occurrence |
| `{n,m}` | Matches between n and m occurrences |
| `( )` | Groups patterns |
| `[ ]` | Defines a character class |
| `\\` | Escapes a special character |


## Functions

| Function | Description |
|----------|-------------|
| `re.findall()` | Returns a list of all matches | 
| `re.search()`  | Returns a Match object if there is a match anywhere in the string |
| `re.split()`   | Returns a list where the string has been split at each match |
| `re.sub()`     | Replaces either one or more matches with a string
| `re.compile()` | Compiles a regex pattern for reuse |
| `re.escape()` | Escapes all special characters in string | ⛑️
| `re.purge()` | Clears the regex cache | 


## Special Sequences

| Symbol | Description |
|--------|-------------|
| `\d` | Matches any digit (0-9) |
| `\D` | Matches any non-digit |
| `\s` | Matches any whitespace character |
| `\S` | Matches any non-whitespace character |
| `\w` | Matches any alphanumeric character |
| `\W` | Matches any non-alphanumeric character |
| `\b` | Matches a word boundary |
| `\B` | Matches a non-word boundary |
| `\A` | Matches the start of a string |
| `\Z` | Matches the end of a string |

## Character Sets

| Pattern | Description |
|---------|-------------|
| `[abc]` | Matches any character in the set |
| `[^abc]` | Matches any character not in the set |
| `[a-z]` | Matches any character in the specified range |
| `[0-9]` | Matches any digit |
| `[a-zA-Z]` | Matches any letter |

## Matching Methods

| Method | Description |
|--------|-------------|
| `re.match()` | Matches pattern at the start of a string |
| `re.fullmatch()` | Matches pattern against entire string |
| `re.search()` | Searches for first occurrence of pattern |
| `re.findall()` | Finds all occurrences of pattern |
| `re.finditer()` | Returns iterator with match objects |
| `re.split()` | Splits string by occurrences of pattern |
| `re.sub()` | Replaces occurrences of pattern |
| `re.subn()` | Replaces occurrences of pattern and returns count |


## Flags

| Flag | Description |
|------|-------------|
| `re.IGNORECASE (re.I)` | Case-insensitive matching |
| `re.MULTILINE (re.M)` | Enables multi-line matching |
| `re.DOTALL (re.S)` | Allows `.` to match newline characters |
| `re.VERBOSE (re.X)` | Allows for readable regex with comments |
| `re.ASCII (re.A)` | Makes `\w`, `\d`, and `\s` match ASCII-only |
| `re.LOCALE (re.L)` | Uses locale-dependent character sets |


