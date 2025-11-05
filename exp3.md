## Experiment 3: Linux File Manipulation and System Manipulation I

### Name:shashwat Agrawal Roll No.: 590029107  Date: 2025-09-23

### Aim:

* To practice Linux file manipulation commands like `touch`, `cp`, `mv`, `rm`, `cat`, `less`, `head`, `tail`.
* To explore file permissions and ownership with `ls -l`, `chmod`, `chown`, and `chgrp`.
* To search and filter files using `find` and `grep`.
* To understand archiving and compression with `tar`, `gzip`, and `gunzip`.
* To create and manage links (`ln`) for both hard and symbolic links.

### Requirements

* A Linux machine with bash shell (Ubuntu/Fedora/other).
* User privileges to create, modify, and delete files and directories.
* Access to system utilities like `tar`, `gzip`, `grep`, and `find`.

## Theory

Linux file management involves creating, copying, moving, removing, and viewing files. File permissions and ownership ensure secure access control. Searching and filtering tools like `grep` and `find` help locate information efficiently. Archiving with `tar` and compression with `gzip` reduce storage usage and simplify file transfer. Links (`ln`) allow multiple references to the same file data (hard links) or path references (symbolic links).

## Procedure & Observations

## Exercise 1: Creating and Managing Files

### Task Statement:

Create files and manage timestamps using `touch`.

### Command(s):

```bash
touch newfile.txt
touch file1.txt file2.txt file3.txt
touch -t 202401151430 dated_file.txt
```

### Output:
<img width="892" height="756" alt="Screenshot 2025-11-06 001808" src="https://github.com/user-attachments/assets/d2d6296e-9a08-4a15-a70c-95c210208e46" />


---

## Exercise 2: Copying, Moving, and Deleting Files

### Task Statement:

Use `cp`, `mv`, and `rm` to copy, rename, move, and delete files and directories.

### Command(s):

```bash
cp document.txt backup_document.txt
mv oldname.txt newname.txt
rm unwanted_file.txt
rm -r old_directory/
```

### Output:

<img width="881" height="664" alt="Screenshot 2025-11-06 002452" src="https://github.com/user-attachments/assets/6bedfd17-8768-444e-920c-7b05291c28a1" />


---

## Exercise 3: Viewing File Contents

### Task Statement:

Display file contents using `cat`, `less`, `head`, and `tail`.

### Command(s):

```bash
cat filename.txt
head -n 5 filename.txt
tail -n 20 filename.txt
```


### Output:

<img width="888" height="674" alt="Screenshot 2025-11-06 002652" src="https://github.com/user-attachments/assets/d7c641f6-0156-4153-a4dc-f8a0c0f5d64b" />


---

## Exercise 4: File Permissions and Ownership

### Task Statement:

Explore file permissions and ownership with `ls -l`, `chmod`, `chown`, and `chgrp`.

### Command(s):

```bash
ls -l
chmod 755 script.sh
chmod u+x script.sh
```

### Output:
<img width="885" height="630" alt="Screenshot 2025-11-06 002818" src="https://github.com/user-attachments/assets/5e1043af-5c5e-4d72-b0fb-3d039d4c2584" />


---

## Exercise 5: File Searching with `find`

### Task Statement:

Search files by name, type, size, and permissions using `find`.

### Command(s):

```bash
find /home -name "*.txt"
find /home -type f -size +100M
find /etc -name "*conf*"
find /tmp -type f -empty -delete
```

### Output:

<img width="873" height="814" alt="Screenshot 2025-11-06 003402" src="https://github.com/user-attachments/assets/2172a7ef-59f5-4b36-9cb7-fc8bc7b28b60" />


---

## Exercise 6: Pattern Searching with `grep`

### Task Statement:

Search for patterns in files using `grep`.

### Command(s):

```bash
grep "error" /var/log/syslog
grep -i "Error" logfile.txt
grep -r "function" ~/code/
grep -n "TODO" *.txt
```

### Output:

<img width="887" height="785" alt="Screenshot 2025-11-06 003546" src="https://github.com/user-attachments/assets/f1fb0356-b8a3-4330-9d4d-884f8aa5b5d4" />


---

## Exercise 7: Archiving and Compression

### Task Statement:

Create and extract archives using `tar`, compress and decompress with `gzip`/`gunzip`.

### Command(s):

```bash
tar -czf backup.tar.gz /home/user/documents
tar -xzf backup.tar.gz -C /restore/
gzip largefile.txt
gunzip largefile.txt.gz
```

### Output:

<img width="880" height="716" alt="Screenshot 2025-11-06 003805" src="https://github.com/user-attachments/assets/0f486d11-10c7-4aca-b03b-8f4a2dbe7068" />


---

## Exercise 8: Creating Links

### Task Statement:

Create and test hard and symbolic links using `ln`.

### Command(s):

```bash
echo "Hello" > original.txt
ln original.txt hardlink.txt
ln -s original.txt symlink.txt
ls -li original.txt hardlink.txt symlink.txt
```

### Output:

<img width="893" height="781" alt="Screenshot 2025-11-06 004030" src="https://github.com/user-attachments/assets/af58e25f-3d63-49ee-a01d-bd882ae1dee3" />


---

## Result

* Successfully created, copied, moved, and deleted files.
* Practiced viewing file contents and monitoring logs.
* Explored file permissions and ownership management.
* Used `find` and `grep` to locate and filter data.
* Created archives and compressed files.
* Demonstrated both hard and symbolic links.

## Challenges Faced & Learning Outcomes

* Challenge 1: Accidentally deleted files with `rm` without `-i`. Learned to use `rm -i` for safety.
* Challenge 2: Remembering numeric vs symbolic permissions in `chmod`. Fixed through repeated practice.

### Learning:

* Gained practical skills with file manipulation and permission commands.
* Learned how to efficiently search files and patterns in Linux.
* Understood how to archive and compress files for better storage management.
* Understood differences between hard and symbolic links.

## Conclusion

This experiment provided hands-on experience with core Linux file management, permissions, searching, archiving, and linking. These are foundational skills for effective Linux system administration and daily usage.
