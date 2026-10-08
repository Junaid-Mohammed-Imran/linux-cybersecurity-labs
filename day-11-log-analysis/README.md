Day 11 — Log Analysis

📌 Topics Covered

Topic 1 — System Logs

- Learned that system logs record events happening on a Linux system.
- Used "journalctl" to view system log entries.
- Practiced viewing recent journal entries.

journalctl -n 20

Topic 2 — Authentication Logs

- Learned how to search logs for authentication and user session activity.
- Used "journalctl" with "grep" to find relevant entries.

journalctl | grep -Ei "login|authentication|session"

Topic 3 — Failed Login Attempts

- Learned how to search logs for failed authentication attempts.
- Looked for terms such as "failed", "authentication failure", and "invalid user".

journalctl | grep -Ei "failed|authentication failure|invalid user"

Topic 4 — Finding Suspicious Activity

- Learned how to combine log filtering commands to investigate suspicious authentication activity.
- Used "tail" to view the latest matching entries.

journalctl | grep -Ei "failed|invalid user|authentication failure" | tail -n 20

- Looked for repeated failures and unfamiliar usernames as indicators that may require further investigation.

🛠️ Commands Practiced

journalctl -n 20
journalctl | grep -Ei "login|authentication|session"
journalctl | grep -Ei "failed|authentication failure|invalid user"
journalctl | grep -Ei "failed|invalid user|authentication failure" | tail -n 20

🎯 What I Learned

- How to view Linux system logs.
- How to search logs for authentication activity.
- How to identify failed authentication attempts.
- How to filter logs for potentially suspicious activity.
- How log analysis can help with basic security investigation.

📅 Day

Day 11 of my Cybersecurity Learning Roadmap.

Status: ✅ Completed
