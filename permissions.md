# File permissions

To list all files (including hidden ones) along with their permissions, you can use the `-la` option with the `ls` command. The `-l` option provides detailed information, including permissions, while the `-a` option ensures hidden files are shown.

Here’s the command:

```bash
ls -la /mnt/c/Users/akash/Desktop
```

This will show:

- File permissions
- Number of links
- Owner
- Group
- File size
- Date of last modification
- File/directory names (including hidden ones)

---

To change the permissions of all files and directories in a directory (e.g., the Desktop) in a structured way, we can create a table using `chmod` to adjust permissions. In Linux, file permissions are represented by three sets of users: the owner, the group, and others. Permissions can be set using symbolic or numeric modes.

### Understanding File Permissions
In a table format, permissions are displayed as three characters:
- `r` = read
- `w` = write
- `x` = execute
- `-` = no permission

The permissions for a file or directory are shown as:
```
rwxr-xr-x
```
This means:
- `rwx` for the owner (read, write, execute)
- `r-x` for the group (read, execute)
- `r-x` for others (read, execute)

### Numeric Mode for Permissions
Permissions can be represented by a number:
- `r = 4`
- `w = 2`
- `x = 1`
- `- = 0`

So the numeric values for the permissions above would be:
```
rwxr-xr-x = 755
```

### Table to Change Permissions

Here's a simple table that shows how to change permissions using both symbolic and numeric modes.

| Permissions | Numeric Value | Symbolic Command        | Description                                            |
|-------------|---------------|-------------------------|--------------------------------------------------------|
| **Read-Write-Execute**  | 777           | `chmod 777 <file>`        | Full permissions for owner, group, and others           |
| **Read-Write-Execute (Owner), Read-Execute (Group & Others)** | 755           | `chmod 755 <file>`        | Common for executable files or directories              |
| **Read-Write (Owner), Read (Group & Others)** | 644           | `chmod 644 <file>`        | Common for text files (owner can modify, others can read) |
| **Read-Execute (Owner), Execute (Group & Others)** | 555           | `chmod 555 <file>`        | Owner can read and execute, others can only execute     |
| **Read-Execute (Owner), No permissions for Group/Others** | 500           | `chmod 500 <file>`        | Owner can read and execute, others have no access       |
| **No permissions for anyone** | 000           | `chmod 000 <file>`        | No permissions at all                                  |
| **Read-Write (Owner), No permissions for Group/Others** | 600           | `chmod 600 <file>`        | Owner can read and write, others have no access         |

### Example Commands for Changing Permissions

- To give full permissions to everyone for a file:
  ```bash
  chmod 777 /mnt/c/Users/akash/Desktop/yourfile
  ```

- To make all files in the Desktop folder readable and executable by everyone, but writable only by the owner:
  ```bash
  chmod 755 /mnt/c/Users/akash/Desktop/*
  ```

- To change permissions for all files and directories on your Desktop to `644` (read/write for the owner, read-only for everyone else):
  ```bash
  chmod 644 /mnt/c/Users/akash/Desktop/*
  ```

- To change all directories on your Desktop to `755` (execute permission for directories to allow navigation):
  ```bash
  find /mnt/c/Users/akash/Desktop -type d -exec chmod 755 {} \;
  ```

- To change all files on your Desktop to `644` (read/write for the owner, read-only for others):
  ```bash
  find /mnt/c/Users/akash/Desktop -type f -exec chmod 644 {} \;
  ```

### Recap

You can adjust permissions according to the numeric values or symbolic modes based on your needs. The `chmod` command is flexible, and you can apply it to individual files or use `find` to apply changes recursively.

---

| [all commands](./README.md) |
| --- |