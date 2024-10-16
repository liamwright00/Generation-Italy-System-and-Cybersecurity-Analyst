Regex: pattern to find text.

In Linux, `grep` can utilize regular expressions (regex) for advanced pattern matching. Here are some key points about using `grep` with regex:

### Basic Regex Examples with `grep`:

| **Regex Pattern**   | **Description**                                      | **Example Command**               |
|---------------------|------------------------------------------------------|-----------------------------------|
| `^pattern`          | Matches lines starting with `pattern`.               | `grep "^Start" file.txt`          |
| `pattern$`          | Matches lines ending with `pattern`.                 | `grep "end$" file.txt`            |
| `.*`                | Matches any number of any characters.                | `grep ".*error.*" file.txt`       |
| `pattern1\|pattern2`| Matches either `pattern1` or `pattern2`.             | `grep "cat\|dog" file.txt`        |
| `[abc]`             | Matches any single character within brackets.        | `grep "[aeiou]" file.txt`         |
| `[^abc]`            | Matches any character not within brackets.           | `grep "[^0-9]" file.txt`          |
| `\\d`               | Matches any digit (equivalent to `[0-9]`).           | `grep "\\d+" file.txt`            |
| `\\w`               | Matches any word character (letters, digits).        | `grep "\\w+" file.txt`            |


### Options for Enhanced Regex:

- **`E`**: Enables extended regex (ERE), allowing more complex patterns without backslashes.
    - Example: `grep -E "a|b" file.txt` matches lines containing `a` or `b`.
- **`P`**: Enables Perl-compatible regex (PCRE), which offers advanced features.
    - Example: `grep -P "\\d{2,}" file.txt` matches lines with two or more digits.

Using these patterns and options can enhance your text searching capabilities significantly! Let me know if you need more details on specific regex patterns or examples!