#  Windows Fundamentals

This module introduced me to the Windows operating system and its core components. Since many enterprise environments use Windows, learning how it works is essential for both offensive and defensive cybersecurity roles.

---

##  Why Learn Windows?

- Most real-world corporate systems are Windows-based.
- Many malware attacks and defenses are Windows-specific.
- Blue Team (defensive) and Red Team (offensive) roles often deal with Windows hosts, logs, users, and policies.

---

##  Windows User Accounts

- Two main types of users:
  - **Administrator**: Full control over the system.
  - **Standard User**: Limited permissions, safer for daily use.
- **UAC (User Account Control)** prompts when elevated privileges are needed.
- **Local Users vs Domain Users**:
  - Local users exist only on that machine.
  - Domain users are managed centrally using Active Directory.

---

##  File Structure in Windows

- Drives like `C:\`, `D:\` represent physical or virtual storage.
- Common folders:
  - `C:\Users\` – user-specific folders
  - `C:\Windows\` – OS files
  - `C:\Program Files\` – 64-bit applications
  - `C:\Program Files (x86)\` – 32-bit applications
  - `C:\Temp\` or `%TEMP%` – temporary files

---

##  Windows Settings & Control Panel

- **Settings App**: Modern UI to manage display, updates, accounts, etc.
- **Control Panel**: Legacy but still powerful; used for:
  - Network & Sharing
  - User accounts
  - Administrative tools
- Tools like `msconfig`, `regedit`, and `eventvwr` are also critical for system management and security.

---

##  Windows Services

- Background processes = **services**
- Managed via:
  - `services.msc` GUI
  - Command line using `sc`, `net start`, or `net stop`
- Examples:
  - `wuauserv` – Windows Update
  - `WinDefend` – Windows Defender

---

##  Windows Registry

- A hierarchical database storing system settings and configurations.
- Keys are like folders, values are like files.
- Access using:
  ```bash
  regedit

Example

- `HKEY_LOCAL_MACHINE\SOFTWARE\`
- `HKEY_CURRENT_USER\`

---

##  Authentication & Security

Login methods:

- Username/password
- PIN
- Biometrics (Windows Hello)

Windows uses the **SAM (Security Account Manager)** database to store hashed credentials.

---

##  File Permissions (ACLs)

Windows uses **Access Control Lists (ACLs)** to manage file permissions (read, write, execute).

- To configure via GUI:  
  Right-click → Properties → **Security** tab

- CLI Tool example (PowerShell):

```powershell
icacls C:\example.txt
```

---

##  Windows Defender & Security Tools

###  Built-in Security Tools:

- **Windows Defender** – Built-in antivirus
- **Windows Firewall** – Filters network traffic
- **BitLocker** – Disk encryption
- **Event Viewer** – View security and system logs

---

##  PowerShell & CMD

- **CMD** = Legacy shell
- **PowerShell** = Modern, object-oriented, powerful scripting shell

### Common Commands:

```powershell
whoami              # Show current user
ipconfig /all       # View network interfaces
tasklist            # Show running processes
netstat -ano        # View open network connections
Get-Service         # List services (PowerShell)
Get-Process         # List processes (PowerShell)
```
