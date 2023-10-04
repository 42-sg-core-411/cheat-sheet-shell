# Cheat Sheet: Shell
A cheat sheet for useful shell commands.

## Find

### Find and Replace in Files

To execute a global find-and-replace in all files in the current and sub-directories:

```bash
find . -type f -exec sed -i 's/old phrase/new phrase/g' {} +
```
