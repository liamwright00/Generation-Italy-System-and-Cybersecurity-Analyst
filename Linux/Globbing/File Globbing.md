### File Globbing in Linux

| **Glob Pattern**         | **Description**                                             | **Example**              | **Explanation**                                                                                      |
|--------------------------|-------------------------------------------------------------|--------------------------|------------------------------------------------------------------------------------------------------|
| `*`                      | Matches **any number of characters**, including zero characters. | `*.txt`                  | Matches all files ending with `.txt` (e.g., `file.txt`, `notes.txt`).                                |
| `?`                      | Matches **exactly one character**.                           | `file?.txt`              | Matches files like `file1.txt`, `fileA.txt`, but not `file10.txt` (since `?` matches exactly one character). |
| `[abc]`                  | Matches **any one character** inside the brackets.           | `file[123].txt`          | Matches `file1.txt`, `file2.txt`, or `file3.txt`.                                                    |
| `[a-z]`                  | Matches **any one character** in the specified range.        | `file[a-z].txt`          | Matches `filea.txt`, `fileb.txt`, etc. for any lowercase letter in the range `a` to `z`.             |
| `[!abc]`                 | Matches **any character except** those inside the brackets.  | `file[!123].txt`         | Matches `file4.txt` or `filex.txt` but not `file1.txt`, `file2.txt`, or `file3.txt`.                 |
| `{pattern1,pattern2}`     | Matches **any one of the comma-separated patterns**.         | `file{1,2,3}.txt`        | Matches `file1.txt`, `file2.txt`, or `file3.txt`.                                                    |
| `[!a-z]`                 | Matches **any character outside** the specified range.       | `file[!a-z].txt`         | Matches `file1.txt` or `file3.txt` but not `filea.txt` or `filez.txt`.                               |
| `**`                     | Matches **any number of directories** (used in modern shells like `bash` with `globstar` enabled). | `**/*.txt`          | Matches `.txt` files in the current directory and all subdirectories.                                |
| `file[0-9][0-9]`         | Matches files with **exactly two digits** at the specified positions. | `file[0-9][0-9].txt` | Matches `file01.txt`, `file23.txt`, but not `file1.txt` or `file100.txt`.                            |
| `file{A,B,C}*`           | Matches files that start with `fileA`, `fileB`, or `fileC`, followed by any characters. | `file{A,B,C}*`    | Matches `fileA1.txt`, `fileB_example.txt`, `fileCfoo.txt`.                                           |
| `\\`                     | **Escapes special characters** to treat them literally.      | `file\\*.txt`            | Matches the file literally named `file*.txt` rather than using `*` as a wildcard.                    |

---

### **Explanation of Common Patterns**:

1. **`*` (Asterisk)**:
    
    Matches any number of characters, including none.
    
    - Example: `*.jpg` matches all `.jpg` files.
2. **`?` (Question Mark)**:
    
    Matches exactly one character.
    
    - Example: `file?.txt` matches `file1.txt`, `fileA.txt`, but not `file12.txt`.
3. **`[ ]` (Character Class)**:
    
    Matches any single character inside the brackets.
    
    - Example: `file[1-3].txt` matches `file1.txt`, `file2.txt`, `file3.txt`.
4. **`{ }` (Brace Expansion)**:
    
    Matches one of several options inside the braces.
    
    - Example: `file{1,2,3}.txt` matches `file1.txt`, `file2.txt`, `file3.txt`.
5. **`[! ]` (Negated Character Class)**:
    
    Matches any single character **not** inside the brackets.
    
    - Example: `file[!1-3].txt` matches `file4.txt`, `fileA.txt`, but not `file1.txt`, `file2.txt`, `file3.txt`.
6. **`**` (Double Asterisk)**:
    
    When `globstar` is enabled, matches zero or more directories.
    
    - Example: `**/*.txt` matches all `.txt` files in the current directory and any subdirectories.
7. **Escaping Special Characters**:
    
    Use `\\` to escape special characters so they are treated literally.
    
    - Example: `file\\*.txt` matches a file literally named `file*.txt`, not files with any characters before `.txt`.
