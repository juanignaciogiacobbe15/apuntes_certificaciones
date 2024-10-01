# Introduction to Regular Expressions

- `.`: Represents a single character.
- `^`: Search the beginning of a line.
- `$`: Search the end of a line.
- `[abc]`: Search for specified characters.
- `[^abc]`: Search for other characters, but not these.
- `*`: Match zero or more of the preceding characters or expression.

## Regular Expression Tools

> [!NOTE] `sed`
> The stream editor command can operate on files using regular expressions.


> [!NOTE] `egrep`
> Command that searches a specified file line by line, returning lines that contain a pattern matching a given regular expression. 
> Equivalent to `grep -E`.


> [!NOTE] `fgrep`
> Searches based on string rather than patterns. Also uses file globbing instead of regular expressions.
> Equivalent to `grep -F`.


