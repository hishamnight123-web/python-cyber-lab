# Ethical Hacking Lab – Python Tools

This repository contains a collection of **Python-based ethical hacking / security tools** that I built as part of my **Ethical Hacking Internship at GTech, Palakkad**.

> ⚠️ **Important:**  
> All scripts are for **learning, research and defensive security only**.  
> I do **NOT** encourage or support using these tools on systems you do not own or have permission to test.

---

## 🔍 Contents

The projects in this repository cover:

- System protection and basic monitoring
- DNS and subdomain enumeration
- Password and hash cracking (for strength testing)
- Network and port scanning
- Client–server communication using sockets
- System information collection (for research)
- SSH botnet-style controller (for automation practice)
- FTP and SSH brute force tools (for authentication testing)

Each folder represents one topic or project and contains:

- The **Python source code**
- Logic that I studied as part of my internship work

---

## 🧩 Projects Overview

### 1. Protection Script (`protection/protection.py`)

**Goal:**  
A small “system guard” to monitor or print basic system-related information.

**What I learned:**

- How simple scripts can be used as security helpers
- Basic input/output handling in Python
- Thinking like a security tool: check–report–act

---

### 2. DNS Enumeration (`dns_enum/dns_enum.py`)

**Goal:**  
Enumerate DNS records (like A, NS, MX, CNAME) for a domain.

**What I learned:**

- How DNS works like a phonebook of the internet
- How attackers and defenders gather domain information
- The importance of reconnaissance in penetration testing

---

### 3. Subdomain Enumeration (`subdomain_enum/subdomain_enum.py`)

**Goal:**  
Discover subdomains of a target domain using a wordlist.

**What I learned:**

- How to send repeated HTTP/DNS requests from Python
- Concept of “attack surface” and why subdomains matter
- Basic OSINT and enumeration techniques

---

### 4. Password Cracker (`password_cracking/cracker.py`)

**Goal:**  
Try multiple passwords (from a wordlist or logic) to find weak credentials.

**What I learned:**

- Brute-force methodology and its limitations
- Why strong, unique passwords are critical
- The ethics of password auditing and testing

---

### 5. Hash Cracker (`password_cracking/hash_cracker.py`)

**Goal:**  
Attempt to recover original text from a hash using wordlists.

**What I learned:**

- How hashing is used to protect passwords
- Why weak passwords are still vulnerable even when hashed
- Practical understanding of hash comparison and cracking

---

### 6. Network Scanner (`network_scanning/network_scaner.py`)

**Goal:**  
Scan a network (e.g., `192.168.x.x`) to identify live hosts.

**What I learned:**

- Basics of network discovery and host scanning
- Relationship to tools like Nmap
- How networks are mapped during security assessments

---

### 7. Port Scanner (`network_scanning/port_scanner.py`)

**Goal:**  
Scan open ports on a target IP.

**What I learned:**

- What ports and services are
- How attackers find entry points on a system
- How to use Python sockets to test connectivity

---

### 8. Client–Server Communication  
`client_server/client.py` and `client_server/server.py`

**Goal:**  
Build a simple client–server model using TCP sockets.

**What I learned:**

- How two machines talk over a network
- Socket programming basics (bind, listen, accept, connect, send, receive)
- The foundation for many real-world network tools

---

### 9. Info Stealer (System Info Collector) (`info_stealer/info_stealer.py`)

**Goal:**  
Collect system information such as OS, user, hardware details (for research/learning).

**What I learned:**

- What type of information is valuable to attackers
- Device fingerprinting concepts
- How to collect and print/save system metadata using Python

> 📝 Used only on my own system and lab machines for ethical learning.

---

### 10. SSH Botnet Controller (`ssh_botnet/ssh_botnet.py`)

**Goal:**  
Control multiple SSH clients from a central script (run commands on each).

**What I learned:**

- How SSH automation works
- Managing multiple sessions and storing credentials (for testing)
- The concept of botnets in a controlled, lab environment

---

### 11. Advanced FTP Brute Force (`ftp_bruteforce/advanced_ftp_brute.py`)

**Goal:**  
Attempt multiple username–password combinations against an FTP server.

**What I learned:**

- FTP protocol basics
- Multi-threading and queues in Python to speed up attempts
- Better error handling and timeout logic

---

### 12. Advanced SSH Brute Force (`ssh_bruteforce/advanced_ssh_brute.py`)

**Goal:**  
Perform SSH brute force with features like password generation, threading, and retries.

**What I learned:**

- How to use the `paramiko` library for SSH connections
- Handling timeouts, retries, and different error types
- Importance of secure SSH configurations in real systems

---

### 13. Basic SSH Brute Force (`ssh_bruteforce/ssh_brute.py`)

**Goal:**  
A simpler version of SSH brute forcing used as a starting point.

**What I learned:**

- Step-by-step logic of checking one password at a time
- How to build a simple prototype before an advanced tool
- Understanding the evolution from basic to advanced scripts

---

## 🛠️ Tech Stack

- **Language:** Python 3
- **Libraries used (depending on script):**
  - `socket`
  - `ftplib`
  - `paramiko`
  - `threading` / `queue`
  - `argparse`
  - `itertools`, `string`
  - `json`, `os`, `sys`
  - (and others as needed per script)

---

## 📦 Installation

```bash
# Clone the repository
git clone https://github.com/your-username/ethical-hacking-lab-python.git
cd ethical-hacking-lab-python

# (Optional) Create a virtual environment
python3 -m venv venv
source venv/bin/activate  # on Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt      # if you create and add one
