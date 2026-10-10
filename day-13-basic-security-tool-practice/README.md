📌Day 13 – Basic Security Tool Practice

Objective

Practice combining Linux commands to investigate users, processes, system logs, and basic security-related activity.

Topic 1: Combining Linux Commands

Command used:

whoami && id

What I learned:

- "whoami" displays the current username.
- "id" displays user ID (UID), group ID (GID), and group information.
- "&&" runs the second command if the first command succeeds.

Topic 2: User and Process Investigation

Commands used:

ps aux | head -n 10
ps -p 1 -o pid,user,comm
ps -u root -o pid,comm

What I learned:

- "ps aux" displays running processes.
- "head -n 10" displays the first 10 lines.
- "ps -p 1 -o pid,user,comm" checks details of process ID 1.
- Process ID 1 was "systemd", running as root.
- Having many processes is normal and does not automatically indicate suspicious activity.

Topic 3: Log Investigation

Commands used:

journalctl -n 10
journalctl | grep -Ei "failed|invalid user|authentication failure" | tail -n 10

What I learned:

- "journalctl -n 10" displays the latest 10 system journal entries.
- "grep -Ei" searches for matching terms without case sensitivity.
- "tail -n 10" displays the last 10 matching lines.
- No matching authentication-related entries appeared in my search.

Topic 4: Practical Security Investigation

I reviewed running processes and recent system logs in my Kali Linux virtual machine.

Observations

- The current user was root, with UID 0.
- Process ID 1 was "systemd".
- The visible logs included routine scheduled tasks and a PHP session cleanup service.
- My search returned no matching failed-login or invalid-user entries.

Note: These observations alone do not prove that a system is completely secure.

Topic 5: Findings and Documentation

This practical helped me understand how Linux commands can be combined to investigate system activity and review logs.

Key Takeaways

- Identify the current user and its privileges.
- Inspect running processes.
- Review recent system logs.
- Search logs for specific security-related terms.
- Record findings carefully without assuming that the absence of matching logs means there are no security issues.

Tools Used

- Kali Linux
- Linux terminal
- "whoami"
- "id"
- "ps"
- "journalctl"
- "grep"
- "tail"
- "head"

Status

Day 13 practical completed.
