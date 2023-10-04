# Cheat Sheet: Shell
A cheat sheet for useful shell commands.

## File Operations

### Find Files by Keyword

To find all files with a given keyword (case-sensitive) in the current and sub-directories and display the file name and line:

```bash
grep -r "free_this_file" .
```

To find all files with a given keyword (case-insensitive) in the current and sub-directories and display the file name and line:

```bash
grep -ri "free_this_file" .
```

To find all files with a given keyword (case-sensitive) in the current and sub-directories and display just the file name:

```bash
grep -rl "free_this_file" .
```

### Find and Replace in Files

To execute a global find-and-replace in all files in the current and sub-directories:

```bash
find . -type f -exec sed -i 's/old-phrase/new-phrase/g' {} +
```
