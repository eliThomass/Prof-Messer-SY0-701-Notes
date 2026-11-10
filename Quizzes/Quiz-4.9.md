# Quiz 4.9 — Log Data
*Professor Messer SY0-701 · Section 4.9*

---

### 1. What information does a firewall log usually record about traffic flows?
- [ ] Logon events, policy changes, and running processes
- [ ] Source/destination IP, port numbers, and disposition
- [ ] Routing updates and network authentication issues
- [ ] Phone type, GPS location, and the browser type used

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Source/destination IP, port numbers, and disposition</p>
<p>Security logs in general document every traffic flow, including blocked and allowed flows, exploit attempts, and blocked URL categories.</p>
</details>

---

### 2. What extra detail does an NGFW add to its logs compared to a traditional firewall?
- [ ] Only the source and destination IP addresses
- [ ] The GPS location of every connected user device
- [ ] Routing updates sent from every network switch
- [ ] The application used and URL filtering categories

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The application used and URL filtering categories</p>
<p>NGFW logs can also include anomalies and suspicious data.</p>
</details>

---

### 3. Where would you find application logs on Windows and on Linux/macOS?
- [ ] Event Viewer on Windows, /var/log on Linux/macOS
- [ ] /var/log on Windows, Event Viewer on Linux/macOS
- [ ] System File Checker on Windows, Tripwire on Linux
- [ ] Group Policy on Windows, SELinux on Linux/macOS

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Event Viewer on Windows, /var/log on Linux/macOS</p>
<p>Application logs are specific to each application, and their details can be parsed on the SIEM.</p>
</details>

---

### 4. Which data would you most likely find in endpoint logs?
- [ ] Header details, sending server, and destination address
- [ ] Routing updates and VPN concentrator authentication
- [ ] Logon events, policy changes, and account management
- [ ] Known OS vulnerabilities and the type of attack seen

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Logon events, policy changes, and account management</p>
<p>Attackers often gain access to endpoints, and there's a lot of data there, including system events and processes. Everything rolls up to the SIEM.</p>
</details>

---

### 5. An analyst combines IPS events with endpoint status in the SIEM. What is this an example of?
- [ ] Packet capture analysis
- [ ] Correlation of security events
- [ ] Metadata collection and review
- [ ] Vulnerability scanning of hosts

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Correlation of security events</p>
<p>Endpoint logs are most useful when they're correlated with other security events in the SIEM.</p>
</details>

---

### 6. What do OS-specific security logs often require before being sent to the SIEM?
- [ ] Encryption before they can be read
- [ ] Deletion after every login session
- [ ] Filtering, so not everything is forwarded
- [ ] Conversion into a packet capture file

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Filtering, so not everything is forwarded</p>
<p>OS security logs record events like brute force attempts, file changes, authentication details, and services that were disabled when they shouldn't be, which helps find problems before they happen.</p>
</details>

---

### 7. Which data points are common in IPS/IDS logs?
- [ ] Timestamp, type of attack, and source/destination IP
- [ ] Phone type, GPS location, and the user's job title
- [ ] Routing updates and the access point's channel list
- [ ] Logon events, account changes, and the process list

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Timestamp, type of attack, and source/destination IP</p>
<p>IPS/IDS is usually integrated into an NGFW, and its logs contain info about predefined vulnerabilities like known OS vulnerabilities and generic security events.</p>
</details>

---

### 8. Routing updates and authentication issues would most likely appear in which logs?
- [ ] Application logs
- [ ] Endpoint logs
- [ ] IPS/IDS logs
- [ ] Network logs

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Network logs</p>
<p>Network logs come from switches, routers, access points, and VPN concentrators, and record network changes and security issues.</p>
</details>

---

### 9. What is metadata?
- [ ] Data that describes other data sources
- [ ] Data that has been encrypted at rest
- [ ] Data that is deleted after a scan
- [ ] Data that only exists in the SIEM

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Data that describes other data sources</p>
<p>Examples include email headers, a phone's GPS location, a web user's browser type, and a file's author details.</p>
</details>

---

### 10. The type of phone that took a photo and its GPS location are examples of which metadata?
- [ ] Email metadata
- [ ] Mobile metadata
- [ ] Web metadata
- [ ] File metadata

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Mobile metadata</p>
<p>Web metadata includes the OS, browser type, and IP address. File metadata includes names, addresses, phone numbers, and titles.</p>
</details>

---

### 11. Which is an example of email metadata?
- [ ] The browser type and IP address of the sender
- [ ] The type of phone used and its GPS location
- [ ] The header details and the sending server
- [ ] The file's title and the author's phone number

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The header details and the sending server</p>
<p>Email metadata also includes the destination address.</p>
</details>

---

### 12. A vulnerability scan finds open shares and guest access that should have been disabled. What type of finding is this?
- [ ] Lack of security controls
- [ ] A false negative
- [ ] Misconfigurations
- [ ] Packet filtering

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Misconfigurations</p>
<p>Scans also check for a lack of security controls (no firewall, anti-virus, or anti-spyware) and for real vulnerabilities, especially newer ones.</p>
</details>

---

### 13. Which statement about automated SIEM reports is true?
- [ ] They remove the need for any human review
- [ ] Someone still needs to read the reports
- [ ] They can only be made by third-party tools
- [ ] They're meant for real-time status only

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Someone still needs to read the reports</p>
<p>Most SIEMs include a report generator, and a third-party one can be used if not. Reports may be easy or complex to create, process, and store.</p>
</details>

---

### 14. Which best describes a security dashboard?
- [ ] A full capture of every packet sent across the network in real time
- [ ] Long-term trend analysis covering several years of historical log data
- [ ] A fixed layout that can't be customized by the security team at all
- [ ] Real-time summaries on a single screen, not meant for long-term analysis

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Real-time summaries on a single screen, not meant for long-term analysis</p>
<p>Most SIEMs and reporting systems let you add or remove information so the dashboard shows the most important data.</p>
</details>

---

### 15. You need to identify unknown traffic and verify that packet filtering is working. Which tool gives you the nitty-gritty details?
- [ ] A SIEM dashboard
- [ ] An automated report
- [ ] File metadata
- [ ] A packet capture

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A packet capture</p>
<p>Packet captures, gathered with a utility like Wireshark or built into a device, help solve complex application issues.</p>
</details>

---

### 16. Where do firewall, application, and endpoint logs roll up so they can be parsed and correlated?
- [ ] The SIEM
- [ ] The sandbox
- [ ] The proxy
- [ ] The DLP

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The SIEM</p>
<p>The Security Information and Event Manager collects logs from many sources so security events can be correlated.</p>
</details>
