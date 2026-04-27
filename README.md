# Manual AWS Cloud Infrastructure Deployment

## Project Overview
A manual, end-to-end deployment of an Nginx web server on **AWS EC2** designed to demonstrate core competencies in Cloud Infrastructure, Linux Systems Administration, and Network Security.

## Tech Stack
* **Cloud Platform:** AWS (EC2, VPC, Security Groups)
* **Operating System:** Amazon Linux 2023
* **Web Server:** Nginx
* **Local Environment:** WSL2 (Ubuntu) / Windows Terminal

## Implementation Highlights
* **Service Management:** Configured and hardened the Nginx service using `systemctl` for automated startup and lifecycle management.
* **Security Hardening:** Implemented the "Principle of Least Privilege" (PoLP) by architecting AWS Security Groups to restrict SSH access and manage inbound HTTP traffic on Port 80.
* **Linux Administration:** Managed filesystem permissions (`chown`, `chmod`) and handled package dependencies using the `dnf` package manager.

## Lessons Learned & Troubleshooting
* **Shell Escaping:** Successfully troubleshot Bash history expansion issues when handling special characters (like `!`) in strings using single-quote literal escaping.
* **Kernel Environments:** Gained a deep understanding of the differences between terminal emulators (Git Bash) and native Linux kernels (**WSL2**), choosing the latter for industry-standard compatibility.

## Verification
* **Deployment Status:** Successfully verified via browser and system logs.
* *Note: Instance decommissioned after successful deployment to optimize cloud costs. Screenshots of successful deployment are included in the repository assets.*
