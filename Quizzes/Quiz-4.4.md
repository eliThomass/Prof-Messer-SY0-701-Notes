# Quiz 4.4 — Security Monitoring
*Professor Messer SY0-701 · Section 4.4*

---

### 1. Which of these is an example of an entry point that should be monitored?
- [ ] The office break room schedule
- [ ] Logins, publicly available services, data storage locations, and remote access
- [ ] Only the main firewall
- [ ] Only employee workstations

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Logins, publicly available services, data storage locations, and remote access</p>
<p>The attackers never sleep, so all entry points need monitoring. Status dashboards give the status of all systems at a glance.</p>
</details>

---

### 2. When monitoring applications, what could a sudden increase or decrease in data transfers indicate?
- [ ] A scheduled patch
- [ ] Improved uptime
- [ ] Data exfiltration
- [ ] A new user account

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Data exfiltration</p>
<p>Application monitoring also covers availability (uptime and response times) and security notifications.</p>
</details>

---

### 3. Logins from strange locations would be caught by monitoring which area of a system?
- [ ] Authentication
- [ ] Server backups
- [ ] Software versions
- [ ] Firewall rule base

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Authentication</p>
<p>System monitoring includes authentication (logins from strange places) and server monitoring (service activity, backups, software versions).</p>
</details>

---

### 4. Which items fall under infrastructure monitoring?
- [ ] Application uptime and response times
- [ ] Device driver versions only
- [ ] Mobile device screenshots
- [ ] Remote access systems and firewall/IPS reports

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Remote access systems and firewall/IPS reports</p>
<p>Remote access systems cover employees, vendors, and guests. Firewall and IPS reports show increases in attacks or the type of attack.</p>
</details>

---

### 5. What is the main purpose of a SIEM?
- [ ] To encrypt data at rest
- [ ] To consolidate many different logs into a central database for reporting and correlation
- [ ] To replace the firewall
- [ ] To assign IP addresses to devices

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> To consolidate many different logs into a central database for reporting and correlation</p>
<p>A Security Information and Event Manager aggregates logs from servers, firewalls, VPN concentrators, SANs, and cloud services, and correlates data across diverse systems.</p>
</details>

---

### 6. Which of these is NOT a typical SIEM capability?
- [ ] Log aggregation and long-term storage
- [ ] Data correlation
- [ ] Forensic analysis
- [ ] Physically destroying old hard drives

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Physically destroying old hard drives</p>
<p>A SIEM provides log collection of security alerts, log aggregation and long-term storage, a reporting engine, data correlation, and forensic analysis.</p>
</details>

---

### 7. When actively scanning systems as part of security monitoring, what kind of information is gathered?
- [ ] OS types and versions, device driver versions, installed apps, and potential anomalies
- [ ] Only employee names
- [ ] Only the device's purchase price
- [ ] Only the number of open tickets

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> OS types and versions, device driver versions, installed apps, and potential anomalies</p>
<p>The threat landscape is constantly changing, so systems and devices are actively checked to gather the raw details.</p>
</details>

---

### 8. Which is an example of the status information a security report might include?
- [ ] The number of devices not up to date or in compliance
- [ ] The color of each server rack
- [ ] Employee lunch schedules
- [ ] The vendor's stock price

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The number of devices not up to date or in compliance</p>
<p>Reporting analyzes the collected data, such as devices running older OS versions, to determine the best next steps. Ad hoc summaries can also be produced.</p>
</details>

---

### 9. Why is archiving security data over an extended period important?
- [ ] It speeds up the network
- [ ] It removes the need for alerting
- [ ] It takes an average of about 9 months to identify and contain a breach, so access to older data is critical
- [ ] Logs are only useful for one day

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It takes an average of about 9 months to identify and contain a breach, so access to older data is critical</p>
<p>There may also be a mandate to archive, from state or federal law or organization requirements.</p>
</details>

---

### 10. Which of these would typically trigger a real-time security alert?
- [ ] A user changing their desktop wallpaper
- [ ] An increase in authentication errors or a large file transfer
- [ ] A scheduled weekly report
- [ ] A printer running low on toner

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> An increase in authentication errors or a large file transfer</p>
<p>Alerts provide actionable data that keeps the right people informed, enabling quick response. Notifications can be sent by SMS/text, email, or the security console.</p>
</details>

---

### 11. What is the foundational security response to an alert, which prevents a security issue from spreading?
- [ ] Alert tuning
- [ ] Archiving
- [ ] Quarantining the system
- [ ] Rebooting the SIEM

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Quarantining the system</p>
<p>Quarantine isolates the affected system so the issue can't spread to the rest of the network.</p>
</details>

---

### 12. What is the goal of alert tuning?
- [ ] To send every alert to every employee
- [ ] To disable all alerts
- [ ] To make alerts louder
- [ ] To balance alerting so you prevent both false positives and false negatives

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> To balance alerting so you prevent both false positives and false negatives</p>
<p>Alert tuning is a balancing act: too sensitive creates false positives, too loose lets real events slip by as false negatives.</p>
</details>

---

### 13. What problem does SCAP (Security Content Automation Protocol) solve?
- [ ] Different security tools each evaluate threats their own way; SCAP gives them a shared language and criteria
- [ ] It encrypts network traffic between firewalls
- [ ] It replaces the need for vulnerability scanners
- [ ] It assigns asset tags to devices

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Different security tools each evaluate threats their own way; SCAP gives them a shared language and criteria</p>
<p>NGFWs, IPSs, and vulnerability scanners all evaluate threats differently. SCAP lets them identify and act on the same criteria and consolidates duplicate vulnerability reports.</p>
</details>

---

### 14. Which of these can tools do using SCAP's shared criteria?
- [ ] Generate new encryption keys
- [ ] Validate security configs, confirm patch installs, and scan for a security breach
- [ ] Print physical reports only
- [ ] Manage employee payroll

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Validate security configs, confirm patch installs, and scan for a security breach</p>
<p>Because the tools share a common language, they can work together on these tasks.</p>
</details>

---

### 15. Where is SCAP especially useful?
- [ ] A single home computer
- [ ] An air-gapped calculator
- [ ] Large environments with many different operating systems and apps
- [ ] Networks with only one type of device

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Large environments with many different operating systems and apps</p>
<p>SCAP content can be shared between tools, and the standard enables automation, even between different tools.</p>
</details>

---

### 16. Which automation types does SCAP enable?
- [ ] Ongoing monitoring, notification and testing, and remediation of noncompliant systems
- [ ] Only manual remediation
- [ ] Only hardware procurement
- [ ] Only password resets

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Ongoing monitoring, notification and testing, and remediation of noncompliant systems</p>
<p>All of these can happen automatically once the tools share SCAP content.</p>
</details>

---

### 17. What is a security benchmark?
- [ ] A speed test for network hardware
- [ ] A set of security best practices giving the bare minimum security settings for OSs, cloud providers, mobile devices, etc.
- [ ] A score from 0–10 for a vulnerability
- [ ] A type of malware

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A set of security best practices giving the bare minimum security settings for OSs, cloud providers, mobile devices, etc.</p>
<p>Benchmarks apply security best practices to everything.</p>
</details>

---

### 18. Which of these is an example of a mobile device benchmark setting?
- [ ] Allow screen recordings
- [ ] Allow voice calls when locked
- [ ] Disable screenshots and force encrypted backups
- [ ] Disable device encryption

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Disable screenshots and force encrypted backups</p>
<p>Other mobile benchmark examples include disabling recordings and preventing voice calls when the device is locked.</p>
</details>

---

### 19. What is an advantage of an agent-based compliance check over an agentless one?
- [ ] It never needs to be updated
- [ ] It requires no installation
- [ ] It only runs on demand
- [ ] It usually provides more detail and monitors constantly for real-time compliance notifications

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It usually provides more detail and monitors constantly for real-time compliance notifications</p>
<p>The trade-off is that an agent must be installed, maintained, and updated.</p>
</details>

---

### 20. What is a drawback of an agentless compliance check?
- [ ] It requires ongoing updates to an agent
- [ ] It will not inform or alert you when it isn't running
- [ ] It must be permanently installed
- [ ] It can only run on servers

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It will not inform or alert you when it isn't running</p>
<p>Agentless checks run on demand without a formal install and don't require ongoing agent updates.</p>
</details>

---

### 21. How do the terms anti-virus and anti-malware compare today?
- [ ] Anti-virus only stops ransomware
- [ ] Anti-malware only stops worms
- [ ] They are effectively the same
- [ ] Anti-virus is a hardware device

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> They are effectively the same</p>
<p>Anti-virus is the popular term (trojans, worms, macro viruses), while malware refers to the broad category of malicious software.</p>
</details>

---

### 22. What does Data Loss Prevention (DLP) do?
- [ ] Monitors traffic in real time and blocks it if it contains sensitive data like SSNs, credit card numbers, or medical records
- [ ] Backs up data to the cloud
- [ ] Encrypts every file on a disk
- [ ] Deletes old log files

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Monitors traffic in real time and blocks it if it contains sensitive data like SSNs, credit card numbers, or medical records</p>
<p>The goal is to stop the data before the attacker gets it. With so many sources and destinations, multiple DLP solutions are often required.</p>
</details>

---

### 23. In SNMP, what is the MIB?
- [ ] A type of SNMP trap
- [ ] The port SNMP uses
- [ ] The Management Information Base, a database of data on the device
- [ ] A NetFlow collector

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The Management Information Base, a database of data on the device</p>
<p>The MIB contains OIDs (Object Identifiers), which identify the individual pieces of data that can be requested.</p>
</details>

---

### 24. What do OIDs represent in SNMP?
- [ ] Object Identifiers stored in the MIB
- [ ] Open Interface Devices
- [ ] Operating system IDs
- [ ] Outbound Internet Domains

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Object Identifiers stored in the MIB</p>
<p>A monitoring station requests the value of specific OIDs to get stats from servers, firewalls, workstations, switches, and routers.</p>
</details>

---

### 25. Which port and protocol does SNMP use for normal polling?
- [ ] tcp/443
- [ ] udp/162
- [ ] tcp/22
- [ ] udp/161

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> udp/161</p>
<p>The monitoring station polls devices at fixed intervals over udp/161, which can be used to build graphs, such as bytes sent per interval.</p>
</details>

---

### 26. How does an SNMP trap differ from a normal SNMP poll?
- [ ] The trap is configured on the monitored device and sends a message over udp/162 when a threshold is hit
- [ ] The trap is sent by the monitoring station every 5 minutes
- [ ] Traps use tcp/161
- [ ] Traps can only be used on firewalls

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The trap is configured on the monitored device and sends a message over udp/162 when a threshold is hit</p>
<p>For example, if CRC errors increase by 5, the device sends a trap, and the monitoring station can react immediately instead of waiting for the next poll.</p>
</details>

---

### 27. In NetFlow, what are the roles of the probe and the collector?
- [ ] The collector watches traffic; the probe stores the records
- [ ] The probe watches network communication and sends summary records to the collector
- [ ] Both block malicious traffic
- [ ] The probe encrypts traffic; the collector decrypts it

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The probe watches network communication and sends summary records to the collector</p>
<p>NetFlow is a standard way to gather traffic statistics from all traffic flows. A separate reporting app is usually linked to the collector.</p>
</details>

---

### 28. Which report would you most likely get from a NetFlow reporting app?
- [ ] A list of unpatched OS versions
- [ ] A certificate of destruction
- [ ] The top 10 conversations on the network between devices
- [ ] A CVSS score for each vulnerability

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The top 10 conversations on the network between devices</p>
<p>NetFlow focuses on traffic flows: who's talking to whom and how much.</p>
</details>

---

### 29. How does a vulnerability scanner compare to a penetration test?
- [ ] A vulnerability scanner performs actual exploits
- [ ] A vulnerability scanner is usually minimally invasive and gathers details on whether a system may be vulnerable
- [ ] They are exactly the same
- [ ] A vulnerability scanner can only test from outside the network

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A vulnerability scanner is usually minimally invasive and gathers details on whether a system may be vulnerable</p>
<p>Scanners do port scans, identify systems and security devices, and test from both outside and inside, but unlike a pentest they don't actually exploit anything.</p>
</details>
