Day 9 — Network Security Commands

📌 Topics Covered

Topic 1 — "ping"

- Learned that "ping" is used to check whether a destination is reachable over a network.
- Learned that "ping" uses ICMP.
- Practiced:

ping -c 4 google.com

- "-c" means count and "4" means send 4 packets.

Topic 2 — "ip"

- Learned that the "ip" command is used to view network interfaces and IP address information.
- Practiced:

ip addr

Topic 3 — "ss"

- Learned that "ss" can display network connections and listening ports.
- Practiced:

ss -tuln

- "-t" — TCP
- "-u" — UDP
- "-l" — Listening
- "-n" — Numeric output

Topic 4 — "netstat"

- Learned that "netstat" can be used to view network connections and listening ports.
- Practiced:

netstat -tuln

Topic 5 — "traceroute"

- Learned that "traceroute" shows the network path between a computer and a destination.
- Learned that each number represents a network hop.
- Practiced:

traceroute google.com

🎯 What I Learned

- How to check network reachability using "ping".
- How to view IP and interface information using "ip".
- How to inspect network connections and listening ports using "ss".
- How to use "netstat" for network information.
- How to trace the network path to a destination using "traceroute".

🛠️ Commands Practiced

ping -c 4 google.com
ip addr
ss -tuln
netstat -tuln
traceroute google.com

📅 Day

Day 9 of my Cybersecurity Learning Roadmap.

Status: ✅ Completed
