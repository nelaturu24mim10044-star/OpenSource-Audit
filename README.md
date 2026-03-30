## OSS-AUDIT-24MIM10044

## **Author**

Nelaturu Sai Krishna Reddy | 24MIM10044

## About
This is my Open Source Software (OSS) lab repository for auditing Git on Ubuntu 24.04 (WSL2).

I’m Nelaturu Sai Krishna Reddy (reg no 24MIM10044). In this project, I created a set of shell scripts to:
* Collect basic system information
* Inspect installed packages
* Audit directories and permissions
* Analyze log files for keyword matches
* Generate an open source manifesto interactively

---

## What’s inside

* `script1.sh` - System Identity Report (kernel, distro, uptime, etc.)
* `script2.sh` - FOSS Package Inspector for git
* `script3.sh` - Disk and Permission Auditor for common directories
* `script4.sh` - Log file analyzer (counts keyword matches)
* `script5.sh` - Open Source Manifesto Generator (interactive)
* `manifesto_NelaturuSaiKrishnaReddy.txt` - Example output generated

---

## Tools Used

* Bash (Shell Scripting)
* Ubuntu 24.04 (WSL2)
* Git

---

## How to run the scripts

From the repository directory:

### Make scripts executable (one-time):

chmod +x script1.sh script2.sh script3.sh script4.sh script5.sh

### Run the scripts:

./script1.sh
./script2.sh
./script3.sh

sudo ./script4.sh /var/log/syslog error

If no keyword is provided, it defaults to `error`.

./script5.sh

It will prompt for inputs and generate:
manifesto_.txt

---

## Notes

* Ubuntu is Debian-based, so `dpkg -l` is used instead of `rpm`
* `script4.sh` may require `sudo` to access system log files
* If `lsb_release` is not installed, run:
  sudo apt install lsb-release

---

## Conclusion

This project demonstrates basic system auditing using shell scripting in a Linux environment. It highlights how open source tools can be used to gather system insights, analyze logs, and automate simple administrative tasks.

---
