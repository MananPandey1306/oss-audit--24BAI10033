# Apache Audit - Script Execution Outputs

This document contains simulated terminal outputs for the 5 audit scripts.

---

## 1. System Identity Report (`01-identify.sh`)
```bash
MananPandey1306@ubuntu-server:~/Apache$ ./01-identify.sh
================================================================================
                   Apache AUDIT - SYSTEM IDENTITY                    
================================================================================
Linux Distribution: Ubuntu 22.04.3 LTS
Kernel Version:     5.15.0-89-generic
Current User:       MananPandey1306
Home Directory:     /home/MananPandey1306
System Uptime:      up 2 hours, 45 minutes
Current Date/Time:  Fri Sep 15 14:30:00 UTC 2023
--------------------------------------------------------------------------------
Message: This system runs on Open Source software, providing freedom to study, change, and distribute.
================================================================================
```
---

## 2. FOSS Package Inspector (`02-packages.sh`)
```bash
MananPandey1306@ubuntu-server:~/Apache$ ./02-packages.sh
================================================================================
                   Apache AUDIT - PACKAGE INSPECTOR                 
================================================================================
Status: apache2 is INSTALLED on this Ubuntu 22.04.3 LTS system.
Version: 2.4.52-1ubuntu4.1
--------------------------------------------------------------------------------
FOSS Philosophy Notes:
 - Apache: Apache is a free and open-source cross-platform web server software.
 - Linux: Linux is a family of open-source Unix-like operating systems based on the Linux kernel.
 - MySQL: MySQL is an open-source relational database management system.
 - PHP: PHP is a server-side scripting language used for web development.
================================================================================
```
---

## 3. Disk and Permission Auditor (`03-auditor.sh`)
```bash
MananPandey1306@ubuntu-server:~/Apache$ ./03-auditor.sh
/etc
4096 drwxr-xr-x root
/var/log
4096 drwxr-xr-x root
/var/www
4096 drwxr-xr-x root
/usr/local/apache2
4096 drwxr-xr-x root
```
---

## 4. Log File Analyzer (`04-logs.sh`)
```bash
MananPandey1306@ubuntu-server:~/Apache$ ./04-logs.sh /var/log/syslog error
Found 10 occurrences of 'error' in /var/log/syslog.
Sep 15 14:25:00 ubuntu-server systemd[1]: Started Session 14 of user MananPandey1306.
Sep 15 14:25:00 ubuntu-server systemd[1]: Started Session 15 of user MananPandey1306.
Sep 15 14:25:00 ubuntu-server systemd[1]: Started Session 16 of user MananPandey1306.
Sep 15 14:25:00 ubuntu-server systemd[1]: Started Session 17 of user MananPandey1306.
Sep 15 14:25:00 ubuntu-server systemd[1]: Started Session 18 of user MananPandey1306.
```
---

## 5. Open Source Manifesto Generator (`05-manifesto.sh`)
```bash
MananPandey1306@ubuntu-server:~/Apache$ ./05-manifesto.sh
What is your name? MananPandey1306
What is your favorite open-source project? Apache
Why do you contribute to open-source? To give back to the community
My name is MananPandey1306, and I love Apache because To give back to the community. I believe in the power of open-source to change the world.
```