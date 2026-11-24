# Linux Server Health & Log Summary Card (`server-summary.sh`)

A clean, beginner-friendly Linux mini-project designed for a **Killercoda Ubuntu 24.04 (`root@ubuntu`)** environment that exercises all 20 Linux commands (`grep`, `sed`, `awk`, `ls`, `pwd`, `cd`, `mv`, `cp`, `systemctl`, `hostnamectl`, `tr`, `cut`, `uname`, `command -v`, `which`, `type`, `file`, `journalctl`, `systemd`, `jq`) in one practical workflow.

---

## 1. Why You Are Doing This & How It Helps DevOps Teams Daily

* **Why build this:** Every time a DevOps or Cloud Engineer logs into a new or unfamiliar Linux server, they need a quick snapshot of **server identity**, **running services**, **recent system errors**, and **application log health**—without typing 15 separate commands manually.
* **Day-to-day DevOps impact:**
  * Saves 5–10 minutes of repetitive manual checks per server during daily health checks or handoffs.
  * Turns messy raw logs and JSON files into a clean, readable report saved automatically for team sharing.

---

## 2. How It Works (Simple Flow)

```mermaid
flowchart LR
    A[System Info<br/>uname, hostnamectl] --> D[server-summary.sh]
    B[Services & Logs<br/>systemd, systemctl, journalctl] --> D
    C[App Log & JSON<br/>grep, sed, awk, cut, tr, jq] --> D
    D --> E[Save & Backup Report<br/>pwd, cd, ls, cp, mv, file]
