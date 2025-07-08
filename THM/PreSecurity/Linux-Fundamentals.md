#  Linux Fundamentals

This module introduced me to the Linux operating system, a critical part of most servers, tools, and security infrastructure. As a cybersecurity learner, understanding Linux is essential — both for attacking and defending systems.

---

##  Why Linux?

- Linux is used in **most servers**, IoT devices, and security tools.
- Many hacking tools and CTF machines run on Linux.
- Learning Linux helps you:
  - Navigate remote servers via CLI (Command Line Interface)
  - Write scripts for automation
  - Understand how services run

---

##  Linux File System

- Root of all files = `/`
- Key directories:
  - `/home` – user directories  
  - `/etc` – system configuration files  
  - `/bin` – essential user binaries  
  - `/var` – log files  
  - `/tmp` – temporary files  
  - `/root` – root user’s home directory  

---

##  Users and Permissions

- Every file and directory has **owners** and **permissions**.
- Use `ls -l` to view permissions.

###  Permission Example:


- `r` = read  
- `w` = write  
- `x` = execute  

---

##  Common Linux Commands

| Command       | Description                    |
|---------------|--------------------------------|
| `pwd`         | Show current directory         |
| `ls`          | List directory contents        |
| `cd`          | Change directory               |
| `touch`       | Create a new file              |
| `mkdir`       | Create a new directory         |
| `cp`          | Copy files/directories         |
| `mv`          | Move or rename files           |
| `rm`          | Delete files                   |
| `cat`         | View file content              |
| `nano` / `vim`| text editor                    |
| `clear`       | Clear terminal screen          |

---

##  File Search & Inspection

- `find` – Search for files:
```bash
find / -name target.txt 2>/dev/null
```

##  grep – Search Inside Files

Search for a keyword inside a file:

```bash
grep "password" file.txt
```

---

##  File Permissions (chmod)

Change file permissions using:

```bash
chmod 755 script.sh
```
---

##  Switching Users

Switch to another user (e.g. root):

```bash
su root
```

Run commands with root privileges:

```bash
sudo apt update
```

---

##  Package Management

###  Debian-based systems (like Ubuntu):

```bash
sudo apt install nmap
```

###  Red Hat-based systems (like CentOS, Fedora):

```bash
sudo yum install nmap
```

or

```bash
sudo dnf install nmap
```


###  Create compressed `.tar.gz` archive:

```bash
tar -czvf archive.tar.gz folder/
```
