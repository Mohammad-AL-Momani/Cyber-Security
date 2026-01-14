## Day 3: Navigating the File System and Common Commands on Kali Linux

Today, I focused on the basics of navigating the file system in **Kali Linux**. This day was all about getting comfortable with the terminal and understanding how to move around, manage files, and work efficiently using common Linux commands.

---

## Understanding the Command Prompt

On Kali Linux, the terminal prompt usually follows this format:

```
kali@kali:~$
```

* **kali** → the username
* **kali** → the hostname
* **~** → the current directory (home directory)
* **$** → indicates a normal user (not root)

This prompt gives you quick context about where you are and who you are logged in as.

---

## The Tilde (~)

The tilde (`~`) represents the **home directory** of the current user. No matter where you are in the file system, using `~` allows you to quickly return to your personal workspace.

---

## Essential File System Commands

### `pwd`

Displays the **current working directory**. It’s basically a way to check your exact location in the file system.

```
pwd
```

---

### `cd`

Used to **change directories**.

Examples:

```
cd /etc
cd ..
cd ~
```

* `cd ..` moves one level up
* `cd ~` takes you back to your home directory

---

### `ls`

Lists files and directories in the current location.

Common options:

* `ls -l` → detailed view
* `ls -a` → shows hidden files
* `ls -la` → combines both

---

### `mkdir`

Creates new directories.

```
mkdir test_folder
```

Useful for organizing projects and lab work.

---

### `rmdir`

Removes **empty** directories.

```
rmdir test_folder
```

---

### `cp`

Copies files or directories.

```
cp file.txt backup.txt
cp -r folder1 folder2
```

The `-r` option is used for copying directories recursively.

---

### `rm`

Deletes files or directories.

```
rm file.txt
rm -r folder_name
```

⚠️ This command is powerful and permanent—there is no recycle bin.

---

### `mv`

Moves or renames files and directories.

```
mv oldname.txt newname.txt
mv file.txt /tmp/
```

This feels very similar to the **cut / rename** function in Windows.

---

### `locate`

Quickly finds files by name across the system.

```
locate passwd
```

This is extremely useful when you don’t remember where a file is located.

---

### `echo`

Outputs text to the terminal or writes it to a file.

```
echo "Hello Kali" > test.txt
```

This can be used to quickly create or overwrite files with content.

---

### `cat`

Displays the contents of a file.

```
cat test.txt
```

It can also be used with redirection (`>`) to create or overwrite files.

---

### `touch`

Creates an empty file or updates the timestamp of an existing file.

```
touch newfile.txt
```

---

## Manual Pages (`man`)

Whenever I need more details about a command, I use **manual pages**.

```
man ls
```

This provides in-depth documentation and available options for almost any command.

---

## Clearing the Terminal

To clear the terminal screen:

```
Ctrl + L
```

This doesn’t delete anything—it just gives a clean workspace.

---

## Hands-On Practice

To make sure I truly understood these concepts, I practiced every command directly on **Kali Linux**. I navigated through directories, checked paths, listed files (including hidden ones), created and deleted folders, copied and moved files, and viewed file contents entirely from the terminal.

This day really helped me feel more confident working in a Linux environment and laid a solid foundation for everything that comes next.

---

*I studied this content as part of my learning journey using Kali Linux.*
