# SOC-Analyst-Lab-Linux-Forensics
"A practical incident response and threat hunting lab simulating multi-stage attacks inside a Kali Linux VM. Features advanced log carving (grep/awk), network analysis (tcpdump/tshark), and active endpoint containment (iptables)."
 Moving beyond theory: I just finished a rigorous, deep-dive hands-on Linux Incident Response and Threat Hunting lab! 

As I train for Tier 1/2 SOC Analyst roles, I wanted to shift from passive collection to active, tactical command-line engineering inside a Kali Linux VM. Here is a quick breakdown of what I executed:

1️⃣ Traffic Triage: Used tcpdump and tshark to parse network layers, hunting for anomalies. Verified the strict baseline differences between routine web activity and automated nmap sweeps by analyzing TCP SYN/RST headers.
2️⃣ Host Correlation: Monitored real-time system logs (journalctl) during a simulated hydra brute-force attack to understand PAM tracking rules and log architecture stability.
3️⃣ Reverse Shell Hunting: Simulated an active outbound reverse shell backdoor. Used lsof -i to hunt down the malicious process by auditing File Descriptors bound directly to active network streams.
4️⃣ Tactical Containment: Built an automated awk log-carving pipeline to dynamically isolate the threat actor's IP, then wrote strict iptables firewall drop rules to achieve immediate 100% packet loss containment.

Documentation and reproducible playbooks are a core part of an analyst's daily workflow, so I have uploaded the complete markdown write-up to my GitHub repository.

Continuous learning is the best defense. Open to any advice or connections from senior practitioners in the blue team space! 

#Cybersecurity #BlueTeam #SOCAnalyst #IncidentResponse #ThreatHunting #Infosec #KaliLinux
