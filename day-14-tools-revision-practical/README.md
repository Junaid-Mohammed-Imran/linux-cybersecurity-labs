📌Day 14 – Tools Revision + Practical

Objective

Revise basic Linux security commands, process analysis, log analysis, and file permissions. Apply the commands in a mini security investigation on my Kali Linux virtual machine.

Topic 1: Linux Security Commands Revision

Commands practiced:

whoami
id
ps aux | head -n 10
ss -tuln
journalctl -n 10

What I Learned

- "whoami" displays the current username.
- "id" displays UID, GID, and group memberships.
- "ps aux" lists running processes.
- "ss -tuln" displays listening TCP and UDP sockets with numerical addresses and ports.
- "journalctl -n 10" displays the latest 10 journal entries.

Topic 2: System and Process Investigation

Commands practiced:

ps aux
top
systemctl --type=service --state=running

What I Learned

- "ps aux" displays running processes.
- "top" provides a live view of processes and resource usage.
- "systemctl" lists running services managed by systemd.
- High CPU or memory usage alone does not prove that a process is malicious.

Topic 3: Log Analysis Revision

Commands practiced:

journalctl -n 10
journalctl | grep -Ei "failed|invalid user|authentication failure" | tail -n 10

What I Learned

- "journalctl" displays system logs.
- "grep -Ei" searches for matching terms without case sensitivity.
- "tail -n 10" displays the last 10 matching lines.
- My authentication-related search returned no output.

Topic 4: File Permission Revision

Commands practiced:

ls -l testfile.txt
chmod 600 testfile.txt

What I Learned

- "ls -l" displays file permissions and ownership.
- "chmod 600" gives the owner read and write permissions while removing permissions for the group and others.
- The permission format "-rw-r--r--" means the owner can read and write, while the group and others can only read.

Topic 5: Mini Security Investigation

Commands used:

whoami && id
ps aux | head -n 10
ps -p 1 -o pid,user,comm
journalctl -n 10
journalctl | grep -Ei "failed|invalid user|authentication failure" | tail -n 10

Findings

1. Current user: "root".
2. PID 1 process: "systemd".
3. Authentication-related search: No matching output was returned.
4. Recent journal entries were reviewed to observe system activity.

Note: These observations do not prove that the system is completely secure. The absence of matching log entries does not rule out security issues.

Tools Used

- Kali Linux
- Linux terminal
- "whoami"
- "id"
- "ps"
- "top"
- "systemctl"
- "ss"
- "journalctl"
- "grep"
- "tail"
- "chmod"

Key Takeaways

- Review users and privileges.
- Inspect processes and running services.
- Search system logs for security-related events.
- Understand basic file permissions.
- Record findings carefully without jumping to conclusions.

Status

Day 14 – Tools Revision + Practical: Completed.
