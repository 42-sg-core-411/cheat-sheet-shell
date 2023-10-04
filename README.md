# Cheat Sheet: Shell
A cheat sheet for useful shell commands.

## File Operations

### Find Files by Keyword

To find all files with a given keyword (case-sensitive) in the current and sub-directories and display the file name and line:

```bash
grep -r "keyword" .
```

To find all files with a given keyword (case-insensitive) in the current and sub-directories and display the file name and line:

```bash
grep -ri "keyword" .
```

To find all files with a given keyword (case-sensitive) in the current and sub-directories and display just the file name:

```bash
grep -rl "keyword" .
```

### Find and Replace in Files

To execute a global find-and-replace in all files in the current and sub-directories:

```bash
find . -type f -exec sed -i 's/old-phrase/new-phrase/g' {} +
```
