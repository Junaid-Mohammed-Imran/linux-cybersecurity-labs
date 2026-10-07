Day 10 — System & Process Analysis

📌 Topics Covered

Topic 1 — Running Processes

- Learned what a process is.
- Learned that every process has a unique Process ID (PID).
- Used "ps aux" to view detailed information about running processes.
- Practiced identifying:
  - User
  - PID
  - CPU usage
  - Memory usage
  - Process/command name

ps aux

Topic 2 — Services

- Learned what system services are.
- Learned that services run in the background and provide functions to the system.
- Used "systemctl" to view currently running services.

systemctl --type=service --state=running

Topic 3 — Resource Usage

- Learned how to monitor CPU and memory usage.
- Used "top" to monitor running processes in real time.
- Practiced identifying:
  - CPU usage
  - Memory usage
  - PID
  - Process name

top

Topic 4 — Identifying Suspicious Processes

- Learned how to inspect processes based on CPU usage.
- Used a command to sort processes by highest CPU usage.

ps aux --sort=-%cpu | head

- Learned that unusually high resource usage can be a reason to investigate a process further.

🛠️ Commands Practiced

ps aux
systemctl --type=service --state=running
top
ps aux --sort=-%cpu | head

🎯 What I Learned

- How to view and identify running processes.
- How to check running system services.
- How to monitor CPU and memory usage.
- How to investigate processes using high CPU resources.
- Basic understanding of process analysis for security monitoring.

📅 Day

Day 10 of my Cybersecurity Learning Roadmap.

Status: ✅ Completed
