# Links

A **link** in UNIX/Linux is a pointer that maps a filename to an underlying file or directory on the storage drive. 

There are two primary types of links:

### 1. Soft Links (Symbolic Links)
A **soft link** is a shortcut that contains only the path string of the target file. If the original file is moved or deleted, the soft link breaks and becomes a "dangling" link. 
* **Command to create:**
```bash
ln -s [original_filename] [link_name]
```

### 2. Hard Links
A **hard link** is a direct reference to the physical file on the storage drive, sharing the exact same **inode number** as the original file. It remains fully valid and accessible even if the original filename is moved or deleted.
* **Command to create:**
```bash
ln [original_filename] [link_name]
```

---

### Verifying Links in the Terminal

* **`ls -i`**: Displays the **inode number** of files. Files that are hard-linked together will display the exact same inode number.
* **`ls -l`**: Displays the file details. For hard links, the **second column** indicates the total number of hard links pointing to that same file content. For soft links, the file permission column starts with an `l` and shows the path arrow pointing to the target file.
