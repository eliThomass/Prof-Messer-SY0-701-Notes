# Quiz 2.5 — Segmentation and Access Control
*Professor Messer SY0-701 · Section 2.5*

---

### 1. Which of the following is NOT one of the reasons for segmenting a network?
- [ ] Performance, such as isolating high-bandwidth apps
- [ ] Security, such as keeping users from talking directly to database servers
- [ ] Compliance, such as mandated segmentation
- [ ] Removing the need for any firewall rules

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Removing the need for any firewall rules</p>
<p>Networks are segmented (physically with devices, logically with VLANs, or virtually) for performance, security, and compliance. Mandated segmentation also makes change control easier.</p>
</details>

---

### 2. What can an access control list (ACL) use to allow or disallow traffic?
- [ ] Only the source IP address
- [ ] Groupings of categories like source IP, destination IP, port number, time of day, and application
- [ ] Only the username of the person logged in
- [ ] Only the MAC address of the switch

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Groupings of categories like source IP, destination IP, port number, time of day, and application</p>
<p>ACLs allow or disallow traffic based on these categories, and can restrict access to network devices by IP address or other ID to prevent non-admin access. Many operating systems also use ACLs to control access to files.</p>
</details>

---

### 3. "James can access 192.168.1.0/24 using TCP ports 80, 443, and 8088" is an example of what?
- [ ] An application deny list
- [ ] An access control list (ACL) rule
- [ ] A posture assessment
- [ ] A host-based IPS signature

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> An access control list (ACL) rule</p>
<p>ACL entries define who can access what, such as "Bob can read files" or "Fred can access the network." Be careful when configuring them!</p>
</details>

---

### 4. Which application control approach means nothing runs unless it's approved?
- [ ] Deny list
- [ ] Allow list
- [ ] Least privilege
- [ ] Network zone

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Allow list</p>
<p>An allow list is very restrictive since only approved apps can run. A deny list is more flexible: anything on the list can't run (this is how anti-virus and anti-malware work).</p>
</details>

---

### 5. An application allow list that only permits apps matching a specific unique identifier is using which method?
- [ ] Certificate
- [ ] Path
- [ ] Application hash
- [ ] Network zone

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Application hash</p>
<p>Allow/deny list examples include application hash (a unique identifier), certificate (digitally signed apps from certain publishers), path (only run apps in certain folders), and network zone (apps can only run from a certain zone).</p>
</details>

---

### 6. Allowing only digitally signed apps from certain publishers to run is which type of allow list rule?
- [ ] Path
- [ ] Certificate
- [ ] Application hash
- [ ] Network zone

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Certificate</p>
<p>A certificate-based rule allows apps that are digitally signed by trusted publishers.</p>
</details>

---

### 7. Why might auto-updating patches not always be the best option in a large organization?
- [ ] Auto-updates never install security fixes
- [ ] Large organizations need to test patches before deploying them
- [ ] Auto-updates only work on third-party apps
- [ ] Patches are only released once a year

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Large organizations need to test patches before deploying them</p>
<p>Patching is incredibly important — monthly updates, third-party updates (app devs, device drivers), and emergency out-of-band updates. But large organizations often need to test patches first.</p>
</details>

---

### 8. What is the difference between file system encryption (like Windows EFS) and full disk encryption (like BitLocker)?
- [ ] EFS encrypts everything on the drive; BitLocker only encrypts individual files
- [ ] File system encryption protects individual files/data; full disk encryption encrypts everything on the drive
- [ ] They're the same thing with different names
- [ ] FDE only encrypts network traffic

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> File system encryption protects individual files/data; full disk encryption encrypts everything on the drive</p>
<p>File system encryption (Windows EFS) prevents access to application data files, FDE (BitLocker, FileVault) encrypts the entire drive, and application data encryption is managed by the app itself.</p>
</details>

---

### 9. In security monitoring, what is a SIEM?
- [ ] A type of host-based firewall
- [ ] A Security Information and Event Manager that collects data from sensors, often with a correlation engine to compare diverse data
- [ ] A tool for scanning open ports
- [ ] An endpoint agent that blocks unknown processes

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A Security Information and Event Manager that collects data from sensors, often with a correlation engine to compare diverse data</p>
<p>Monitoring aggregates info from sensors (IPS, firewall logs, auth logs, web server access logs, DB logs, email logs) into collectors like a SIEM.</p>
</details>

---

### 10. Which principle says rights and permissions should be set to the bare minimum needed to complete a task?
- [ ] Defense in depth
- [ ] Least privilege
- [ ] Posture assessment
- [ ] Segmentation

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Least privilege</p>
<p>With least privilege, all user accounts are limited, apps run with minimal privileges, and users aren't allowed to run with admin privileges.</p>
</details>

---

### 11. What happens during a posture assessment when a device connects or logs in?
- [ ] The device is automatically given admin rights
- [ ] An extensive check of things like OS patch version, EDR version, firewall/EDR status, and certificate status
- [ ] The device's hard drive is wiped
- [ ] Only the username and password are verified

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> An extensive check of things like OS patch version, EDR version, firewall/EDR status, and certificate status</p>
<p>A posture assessment is part of configuration enforcement and happens each time a device connects or logs in.</p>
</details>

---

### 12. What happens to a system that fails a posture assessment and is out of compliance?
- [ ] It's permanently banned from the network
- [ ] It's quarantined on a private VLAN until changes are made
- [ ] It's given full access anyway
- [ ] Its user account is deleted

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It's quarantined on a private VLAN until changes are made</p>
<p>Systems out of compliance are quarantined and moved to a private VLAN until they're brought back into compliance.</p>
</details>

---

### 13. What is the right approach to decommissioning storage drives?
- [ ] Throw them in the trash
- [ ] Follow a formal policy to recycle or destroy them, so no one finds the data
- [ ] Sell them online without wiping
- [ ] Keep them in an unlocked storage closet

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Follow a formal policy to recycle or destroy them, so no one finds the data</p>
<p>Decommissioning should be a formal policy, usually for storage drives. Don't just throw data in the trash for someone to find.</p>
</details>

---

### 14. Which of the following is a system hardening technique?
- [ ] Giving all users admin rights
- [ ] Applying OS updates, service/security packs, and patches, plus enforcing a password policy
- [ ] Opening all ports for convenience
- [ ] Disabling anti-virus to improve performance

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Applying OS updates, service/security packs, and patches, plus enforcing a password policy</p>
<p>System hardening is many and varied: OS updates and patches, password policies, account limitations (least privilege), limited network access, and monitoring/securing with anti-virus.</p>
</details>

---

### 15. Which two methods are used to encrypt all network communication as a hardening technique?
- [ ] EFS and BitLocker
- [ ] VPN and application encryption (HTTPS)
- [ ] Nmap and SIEM
- [ ] ACLs and VLANs

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> VPN and application encryption (HTTPS)</p>
<p>Network communication can be encrypted with a Virtual Private Network (VPN) or with application-level encryption like HTTPS.</p>
</details>

---

### 16. Why is endpoint protection described as "multi-faceted"?
- [ ] It only protects inbound traffic
- [ ] The endpoint is the user's access to apps and data across many platforms, so it uses defense in depth to stop attackers inbound and outbound
- [ ] It relies on a single anti-virus product
- [ ] It's only needed on servers

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The endpoint is the user's access to apps and data across many platforms, so it uses defense in depth to stop attackers inbound and outbound</p>
<p>The endpoint is where users access apps and data, so protection is layered (defense in depth).</p>
</details>

---

### 17. Besides signatures, how can Endpoint Detection and Response (EDR) detect a threat?
- [ ] Only by waiting for a user to report it
- [ ] With behavioral analysis, machine learning, and process monitoring via a lightweight agent
- [ ] By scanning for open ports with Nmap
- [ ] By checking the device's certificate status

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> With behavioral analysis, machine learning, and process monitoring via a lightweight agent</p>
<p>EDR detects threats, investigates them with root cause analysis, and responds by isolating the system, quarantining the threat, or rolling back to a previous config.</p>
</details>

---

### 18. What makes EDR's response process different from traditional anti-virus?
- [ ] It requires a technician to approve every action
- [ ] It's API driven and can isolate, quarantine, and roll back automatically with no user or technician required
- [ ] It only creates a log entry
- [ ] It can only respond to known signatures

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It's API driven and can isolate, quarantine, and roll back automatically with no user or technician required</p>
<p>EDR is a different method of threat protection: detect, investigate, and respond, all automated through APIs.</p>
</details>

---

### 19. What does a host-based firewall do?
- [ ] Encrypts the entire hard drive
- [ ] A software-based firewall that allows or disallows incoming/outgoing app traffic and can identify and block unknown processes
- [ ] Manages VLAN assignments across the network
- [ ] Collects logs from every device into one console

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A software-based firewall that allows or disallows incoming/outgoing app traffic and can identify and block unknown processes</p>
<p>A host-based firewall runs as software on the device itself and controls app traffic in both directions.</p>
</details>

---

### 20. Which of these can a Host-based IPS (HIPS) identify?
- [ ] Buffer overflows, registry updates, writing files to the Windows folder, and access to non-encrypted data
- [ ] Only physical intrusions into the building
- [ ] Only expired certificates
- [ ] Only phishing emails

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Buffer overflows, registry updates, writing files to the Windows folder, and access to non-encrypted data</p>
<p>HIPS recognizes and blocks known attacks, secures OS and app configs, and validates incoming service requests, using signatures, heuristics, and behavioral detection.</p>
</details>

---

### 21. What is the recommended approach for open ports and services, and which tool can verify it?
- [ ] Open all ports and verify with a SIEM
- [ ] Close everything except required ports, control access with a firewall, and verify with Nmap
- [ ] Leave defaults in place and verify with EDR
- [ ] Only close ports on weekends

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Close everything except required ports, control access with a firewall, and verify with Nmap</p>
<p>Every open port is a possible entry point, so close everything that isn't required.</p>
</details>

---

### 22. Besides changing default passwords on a network device's management interface, what extra security is recommended?
- [ ] Disabling the firewall
- [ ] Adding 2FA
- [ ] Sharing the admin password with all users
- [ ] Using the same password on every device

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Adding 2FA</p>
<p>Every network device has a management interface — change the default settings and add extra security like 2FA.</p>
</details>

---

### 23. Why should unused software be removed from a system?
- [ ] It always contains malware
- [ ] All software contains bugs, some of which are vulnerabilities, and keeping every app updated is hard to manage
- [ ] It's required by the OS license
- [ ] Unused software slows down the network

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> All software contains bugs, some of which are vulnerabilities, and keeping every app updated is hard to manage</p>
<p>Removing all unused software reduces the attack surface and the update burden.</p>
</details>
