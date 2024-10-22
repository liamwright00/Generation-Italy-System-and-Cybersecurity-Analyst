

# Linux Shell Scripting: Conditional Statements

In Linux shell scripting, conditional statements using `if`, `then`, `else`, and `fi` allow you to control the flow of execution based on certain conditions.

## Syntax

1. **Basic `if` Statement:**

    ```bash
    if [ condition ]; then
        # commands to execute if the condition is true
    fi
    ```

2. **`if-else` Statement:**

    ```bash
    if [ condition ]; then
        # commands to execute if the condition is true
    else
        # commands to execute if the condition is false
    fi
    ```

3. **`if-elif-else` Statement:**

    ```bash
    if [ condition1 ]; then
        # commands to execute if condition1 is true
    elif [ condition2 ]; then
        # commands to execute if condition2 is true
    else
        # commands to execute if none of the conditions are true
    fi
    ```

---

## Common Conditions

Here are some common types of conditions that you can use in shell scripting:

### File Tests
- `-e filename`: True if the file exists.
- `-f filename`: True if the file is a regular file.
- `-d directory`: True if the directory exists.
- `-r filename`: True if the file is readable.
- `-w filename`: True if the file is writable.
- `-x filename`: True if the file is executable.

### String Tests
- `-z string`: True if the string is null (empty).
- `-n string`: True if the string is not null.
- `string1 = string2`: True if the strings are equal.
- `string1 != string2`: True if the strings are not equal.

### Numeric Tests
- `num1 -eq num2`: True if the numbers are equal.
- `num1 -ne num2`: True if the numbers are not equal.
- `num1 -lt num2`: True if `num1` is less than `num2`.
- `num1 -le num2`: True if `num1` is less than or equal to `num2`.
- `num1 -gt num2`: True if `num1` is greater than `num2`.
- `num1 -ge num2`: True if `num1` is greater than or equal to `num2`.

---

## Example Script

Below is an example script that demonstrates how to use conditional statements in Linux shell scripting.

```bash
#!/bin/bash

# Prompt the user to enter a number
echo "Enter a number:"
read number

# Check if the number is positive, negative, or zero
if [ $number -gt 0 ]; then
    echo "$number is positive."
elif [ $number -lt 0 ]; then
    echo "$number is negative."
else
    echo "$number is zero."
fi
```

### Explanation:

1. The script asks the user to enter a number using `read`.
2. It uses an `if-elif-else` statement to check if the number is:
   - Greater than 0 (positive).
   - Less than 0 (negative).
   - Equal to 0 (zero).
3. Based on the condition, it outputs the appropriate message.



