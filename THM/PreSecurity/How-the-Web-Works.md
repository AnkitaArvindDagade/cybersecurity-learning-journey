#  How the Web Works

This module introduced me to how the internet and websites actually function behind the scenes — which is essential knowledge for any aspiring hacker or cybersecurity professional.

---

##  Key Concepts

###  The Internet

- The Internet is a **network of networks**, allowing devices across the world to communicate.
- Your device connects to other devices (like web servers) via the internet using **IP addresses**.

###  Clients & Servers

- **Client**: The user’s device (like a browser) that requests content.
- **Server**: The machine that hosts the content (like a website) and sends the response back.
- Communication happens using the **HTTP** or **HTTPS** protocols.

###  HTTP vs HTTPS

- **HTTP (Hypertext Transfer Protocol)**: A protocol used to transfer data.
- **HTTPS** is the secure version (encrypted using SSL/TLS).
- Websites with HTTPS provide **confidentiality, integrity, and authenticity**.

---

##  DNS (Domain Name System)

- DNS translates **domain names** (like `tryhackme.com`) into **IP addresses**.
- Like a phonebook — humans remember names, machines use IPs.
- Example: `tryhackme.com → 104.20.59.209`

---

##  Web Requests

When a client visits a website:
1. It sends a **request** to the server.
2. The server **responds** with the requested content (like HTML, CSS, JavaScript files).
3. The browser renders this data visually for the user.

---

##  Useful Tools

###  Developer Tools (Browser)

- **Inspect Elements**: View the structure of a webpage.
- **Network Tab**: Monitor the requests made by the browser to the server.
- **Console**: Debug and interact with JavaScript.

---

##  Why This Is Important in Cybersecurity

- Understanding how the web works helps you understand:
  - How attackers exploit websites (e.g., via insecure HTTP, broken authentication).
  - How to identify and mitigate security flaws in web apps.
  - Tools like Burp Suite, which rely on intercepting HTTP(S) traffic.

---

##  Summary

This module helped build my foundation in:
- Client-server architecture
- Web request/response lifecycle
- HTTP/HTTPS protocols
- DNS and IP communication

Understanding these basics is critical before diving into web hacking or bug bounty hunting.

