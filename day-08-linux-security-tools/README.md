Day 8 — Linux Security Tools

📌 Topics Covered

Topic 1 — Processes

- Learned what a process is.
- Used "ps" to view running processes.
- Learned that every process has a Process ID (PID).

Topic 2 — Users & Logged-in Users

- Used "whoami" to identify the current user.
- Used "who" to view currently logged-in users.
- Learned about Linux users and user identification.

Topic 3 — File Permissions

- Learned Linux file permissions:
  - "r" — Read
  - "w" — Write
  - "x" — Execute
- Learned about:
  - Owner
  - Group
  - Others
- Practiced understanding permissions such as "-rw-r--r--".

Topic 4 — Logs

- Explored the "/var/log" directory.
- Used "journalctl" to view system logs.
- Used "grep" to search logs for failed activity.
- Used "tail" to view the last 10 matching entries.

Example:

journalctl | grep -i "failed" | tail -n 10

Topic 5 — Basic Security Commands

Practiced basic Linux commands useful for security analysis:

id
ps
ss
who
last

- "id" — Displays UID, GID and group information.
- "ps" — Displays running processes.
- "ss" — Displays network connections and listening ports.
- "who" — Shows currently logged-in users.
- "last" — Shows login history.

🔍 Practical Observation

My current Linux user was:

root

My UID was:

0

UID 0 represents the root user, which has the highest level of privileges in Linux.

🎯 What I Learned

- How Linux processes are identified.
- How to identify users and logged-in sessions.
- How Linux file permissions work.
- How to inspect system logs.
- How basic Linux commands can be used for security monitoring and investigation.

🛠️ Commands Practiced

ps
whoami
who
id
ss
last
journalctl
grep
tail

📅 Day

Day 8 of my Cybersecurity Learning Roadmap.

Status: ✅ Completed
