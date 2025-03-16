# Guide for eJPTv2

## Introduction:
In this guide, we will cover 100% practical content to prepare for the eJPTv2. The main technical and pedagogical topics will be presented to apply in the exam and perform at the best level. Ideally, this is for understanding everything that is directly included without delving into concepts or processes.

### Methodology for Taking the Exam:
It is crucial to understand that the exam and certification are based on a real corporate environment. To perform well as a penetration tester, there are phases that apply in most cases, where being organized and patient is key. The phases are as follows:

### 1. Passive and Active Reconnaissance

First phase in which our objective is to gather all information about the target(s). This includes:

    DNS: Identification of domains and subdomains.
    Subdomains: Discovery of subdomains associated with the target.
    Exposed Ports: Identification of open ports and associated services.

### 2. Enumeration

Second phase in which all the gathered information must be analyzed to look for vulnerabilities. This includes:

    Directory Testing: Searching for exposed paths and files.
    Unprotected Databases: Identifying accessible databases.
    Brute Force on Open Services: Brute force attacks on services such as SSH, FTP, etc.

### 3. Exploitation

Third phase in which we take advantage of a vulnerability to gain any type of privileges, such as:

    File Access: Reading or modifying sensitive files.
    Remote Shells: Gaining access to systems through shells.
    Data and Users: Extracting sensitive information or credentials.

### 4. Post-Exploitation

Fourth phase in which, after exploitation, privilege escalation may be necessary depending on the scope. Here, we ask ourselves:

    Does this vulnerability involve other ports or services?
    Could it help us gain access to other targets or sensitive information?

### 5. Documentation

At this stage, we focus on documenting all findings using diagrams and notes. This is crucial for presenting a clear and professional report.
Exam Structure

    Key Topics:
        Networking: Nmap scanning on multiple targets, ping sweep to identify internal networks, open port identification, service version detection for each port, using Nmap scripts to find vulnerabilities, identifying OS of each target, understanding IP structure, subnet mask, stealth scanning, UDP/TCP, understanding services like SMB, FTP, RDP, identifying the most common ports with these services, port forwarding, pivoting.
        Web: Fuzzing, vulnerability detection by version, CMS, XSS, SQL Injection, brute force, and hashes.

    Duration: 48 hours.

    Format: Practical, with scenario-based questions. Includes multiple-choice and dynamic questions.

Example Questions
Multiple-Choice Questions

Example: What is Luciano's password?

    A) lol123
    B) CITT123
    C) telefono
    D) password

Dynamic Questions

Example: What is the content of the file XXXX.txt for user X on X server and X path?

    Enter answer:

### Recommended Resources

    TryHackMe:
        Attached machines in tryhackme.md.
        Junior Penetration Tester path.

    Videos:
        Xerosec Exam Simulation.
        Zunder Exam Simulation.

    Recommended Tools:
    The following tools have been selected based on INE's recommendations, with additional ones that should be sufficient to complete the exam without issues. It is also advisable to know more than one tool for a task due to false positives and different problems that may arise. For example, Hashcat and John.
        Nmap: Port scanning and service detection.
        Dirb: Directory and file enumeration on web servers.
        Nikto: Web server vulnerability scanning.
        WPScan: WordPress site vulnerability scanning.
        CrackMapExec: Windows network auditing tool.
        The Metasploit Framework: Exploit development and execution framework.
        Searchsploit: Exploit searching in the Exploit-DB database.
        Hydra: Brute force tool for network services.
        Hashcat: Hash cracking tool.
        John the Ripper: Another hash cracking tool.
        SQLMap: Automated SQL Injection testing.
        Gobuster: Directory and subdomain enumeration.

### Organization Tools:

CherryTree
alt text
A highly recommended tool for structuring information in a simple way without excessive complexity. It also allows for general note-taking and tracking per machine, where a full scan for that machine, ports, services, etc., can be recorded.

Draw.io
alt text
A highly recommended tool for having a topological view of the network and directly noting certain details.

### Tips:

1- The machine provided for the exam may fail, leading to issues such as being unable to exit the editor, scans not completing, and various other problems. If this happens, simply stop the lab and restart it to access the machine again. However, make sure to note everything down, as restarting the machine erases all files.

2- Take your time. Perform the reconnaissance and enumeration phase as thoroughly as possible, testing different Nmap combinations to avoid mistakes in such questions and to prevent having to re-enumerate everything later.

3- Document and take notes on everything. You will be dealing with an environment containing different IPs with numerous services and ports. Being organized and recording all findings is crucial, as this will help later in ruling out certain machines for some questions or confirming them.