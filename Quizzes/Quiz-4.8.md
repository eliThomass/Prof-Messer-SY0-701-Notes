# Quiz 4.8 — Incident Response
*Professor Messer SY0-701 · Section 4.8*

---

### 1. Which items belong under incident analysis resources when preparing for an incident?
- [ ] Laptops, removable media, and digital cameras
- [ ] Clean OS images and clean application images
- [ ] Network diagrams and critical file hash values
- [ ] Phone numbers and other contact information

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Network diagrams and critical file hash values</p>
<p>Analysis resources also include documentation and security baselines. The other options are incident handling hardware, mitigation software, and communication methods.</p>
</details>

---

### 2. Keeping clean OS and application images ready falls under which preparation category?
- [ ] Incident analysis resources
- [ ] Incident mitigation software
- [ ] Communication methods
- [ ] Incident handling hardware and software

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Incident mitigation software</p>
<p>Incident handling hardware and software covers laptops, removable media, forensic software, and digital cameras.</p>
</details>

---

### 3. Why prepare policies for incident handling ahead of time?
- [ ] So incidents can be handled without any tools
- [ ] So everyone knows what to do when one happens
- [ ] So the legal team never has to get involved
- [ ] So that detection becomes fully automatic

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> So everyone knows what to do when one happens</p>
<p>Policies are one part of preparation, alongside communication methods, handling hardware and software, analysis resources, and mitigation software.</p>
</details>

---

### 4. Why is detecting incidents a challenge?
- [ ] Most incidents are simple and need little knowledge
- [ ] Detection tools only report a few alerts per day
- [ ] There are many sources and a large volume of data
- [ ] There is only one place where incidents show up

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> There are many sources and a large volume of data</p>
<p>Incidents are also almost always complex, so extensive knowledge is needed to detect them.</p>
</details>

---

### 5. Which of these is a sign that an attack is already underway?
- [ ] A vendor publishes a new exploit announcement
- [ ] A security team reviews the web server log
- [ ] An attacker group sends a direct threat
- [ ] Network traffic flows deviate from the norm

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Network traffic flows deviate from the norm</p>
<p>Other signs of an attack underway include a buffer overflow attempt, anti-virus identifying malware, and a host-based monitor detecting a config change. Exploit announcements and direct threats suggest an attack could happen.</p>
</details>

---

### 6. A host-based monitor detects an unexpected configuration change on a server. What does this most likely mean?
- [ ] The server needs a new asset tag
- [ ] A legal hold has been issued
- [ ] A tabletop exercise has started
- [ ] An attack may be underway

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> An attack may be underway</p>
<p>A config change detected by a host-based monitor is one of the analysis indicators that an attack is in progress.</p>
</details>

---

### 7. During an incident, what is the general guidance on letting an attack run its course?
- [ ] It's best, since it shows what the attacker wants
- [ ] It's a bad idea, so isolate and contain the attack
- [ ] It's required before any evidence can be gathered
- [ ] It's fine as long as backups are available

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> It's a bad idea, so isolate and contain the attack</p>
<p>It's generally a bad idea to let things run their course. Isolation and containment limit the damage.</p>
</details>

---

### 8. What is a sandbox used for during incident response?
- [ ] Storing evidence under a legal hold
- [ ] Holding clean OS and app images for system recovery
- [ ] Running malware in an isolated OS to analyze it
- [ ] Sending simulated phishing emails to users

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Running malware in an isolated OS to analyze it</p>
<p>When the analysis is done, the sandbox is cleaned out.</p>
</details>

---

### 9. Why can isolating malware in a virtual machine be problematic?
- [ ] VMs can't run the same operating systems as hosts
- [ ] Sandboxes automatically send the malware to users
- [ ] Malware can recognize it's in a VM and delete itself
- [ ] Virtual machines can't be cleaned out after use

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Malware can recognize it's in a VM and delete itself</p>
<p>If the malware removes itself, there's nothing left to analyze.</p>
</details>

---

### 10. Removing malware, disabling breached user accounts, and fixing vulnerabilities are part of which step?
- [ ] Preparation
- [ ] Containment
- [ ] Eradication
- [ ] Recovery

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Eradication</p>
<p>Eradication gets rid of the bug before the system is recovered.</p>
</details>

---

### 11. Restoring from backups, replacing compromised files, and tightening down the new system are part of which step?
- [ ] Recovery
- [ ] Eradication
- [ ] Detection
- [ ] Analysis

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Recovery</p>
<p>Recovery can also mean rebuilding the system from scratch.</p>
</details>

---

### 12. Which is true about the post-incident meeting?
- [ ] Wait several months so emotions can settle first
- [ ] Only hold it if the incident caused data loss
- [ ] Hold it before the incident is fully contained
- [ ] Don't wait too long, and answer the tough questions

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Don't wait too long, and answer the tough questions</p>
<p>Tough questions include: What exactly happened? What should we do differently next time? What indicators warned us?</p>
</details>

---

### 13. What is the correct order of the incident response process?
- [ ] Detection, preparation, recovery, containment, eradication, lessons learned
- [ ] Preparation, detection, analysis, containment, eradication, recovery, lessons learned
- [ ] Preparation, containment, detection, analysis, recovery, eradication, lessons learned
- [ ] Analysis, detection, preparation, eradication, containment, recovery, lessons learned

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Preparation, detection, analysis, containment, eradication, recovery, lessons learned</p>
<p>This order comes from the course and matches the order of your notes. Lessons learned is the post-incident meeting.</p>
</details>

---

### 14. Which is a key part of an incident response exercise?
- [ ] A vague scenario so the team has to improvise
- [ ] Skipping evaluation so the team isn't discouraged
- [ ] Running it only after a real incident has occurred
- [ ] Well-defined rules of engagement and a specific scenario

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Well-defined rules of engagement and a specific scenario</p>
<p>Exercises test you before an actual event, and the response is evaluated afterward.</p>
</details>

---

### 15. Why would an organization run a tabletop exercise instead of a full-scale one?
- [ ] Full-scale exercises can be costly and time consuming
- [ ] Tabletop exercises test the actual production systems
- [ ] Tabletop exercises don't need any of the key players
- [ ] Full-scale exercises can't test incident policies

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Full-scale exercises can be costly and time consuming</p>
<p>Key players sit around a table and step through the policies and procedures for an event, since much of the logistics can be determined through analysis.</p>
</details>

---

### 16. The security team sends a fake phishing email to everyone in the organization. What can this simulation test?
- [ ] Whether backups can be restored within the recovery time
- [ ] Whether a legal hold was correctly issued
- [ ] Whether the email got past the filter and fooled users
- [ ] Whether the sandbox catches malware that detects VMs

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Whether the email got past the filter and fooled users</p>
<p>Simulations test internal security and users, and users who fall for it can get more training. Other simulations include password requests and data breaches.</p>
</details>

---

### 17. How do you find the root cause of an incident?
- [ ] By asking "why" until you reach the ultimate cause
- [ ] By picking the first cause that explains the event
- [ ] By assuming every incident has exactly one cause
- [ ] By relying on the attacker's own explanation

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> By asking "why" until you reach the ultimate cause</p>
<p>Don't get tunnel vision: there can be more than one root cause.</p>
</details>

---

### 18. What should the conclusions of a root cause analysis be based on?
- [ ] The opinions of the most senior staff
- [ ] Assumptions about the attacker's motive
- [ ] The facts gathered about the incident
- [ ] The results of the last tabletop exercise

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The facts gathered about the incident</p>
<p>Root cause analysis produces a set of conclusions about the incident, backed up by the facts.</p>
</details>

---

### 19. Why is threat hunting needed in addition to threat intelligence?
- [ ] Intelligence is reactive, so attacks aren't seen until they happen
- [ ] Intelligence data always predicts attacks well before they happen
- [ ] Threat hunting replaces the need for technology or automation
- [ ] Attacker strategies never change, so hunting is always simple

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Intelligence is reactive, so attacks aren't seen until they happen</p>
<p>Threat hunting means finding the attacker before they find you. Strategies are always changing, so technology and automation help speed up reaction time.</p>
</details>

---

### 20. What are the three steps of the standard digital forensic process?
- [ ] Preparation, containment, and recovery
- [ ] Acquisition, analysis, and reporting
- [ ] Detection, eradication, and lessons learned
- [ ] Collection, encryption, and destruction

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Acquisition, analysis, and reporting</p>
<p>Digital forensics collects and protects information relating to an intrusion. It's detail oriented, so take extensive notes.</p>
</details>

---

### 21. Who initiates a legal hold?
- [ ] The incident response team
- [ ] The system administrator
- [ ] The affected end user
- [ ] Legal counsel

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Legal counsel</p>
<p>A legal hold preserves relevant information to prepare for impending litigation.</p>
</details>

---

### 22. After custodians receive a hold notification, what is their obligation?
- [ ] Delete the data once it has been copied
- [ ] Hand the data straight to the attacker
- [ ] Preserve the data for 30 days only
- [ ] Preserve the data on an ongoing basis

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Preserve the data on an ongoing basis</p>
<p>Once notified, there's an ongoing obligation to preserve the data.</p>
</details>

---

### 23. Under a legal hold, where is electronically stored information (ESI) kept?
- [ ] In a separate repository with its own workflow and retention requirements
- [ ] On the user's own workstation, alongside their normal day-to-day files
- [ ] In the organization's standard backups with the usual retention period
- [ ] In a sandbox that is cleaned out as soon as the analysis is finished

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> In a separate repository with its own workflow and retention requirements</p>
<p>ESI gets a unique workflow and retention requirements separate from normal data.</p>
</details>

---

### 24. How does chain of custody protect evidence from tampering?
- [ ] By encrypting the evidence so nobody can read it
- [ ] By deleting the evidence once the report is done
- [ ] By using hashes and digital signatures to track access
- [ ] By limiting the evidence to a single storage drive

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> By using hashes and digital signatures to track access</p>
<p>Chain of custody controls evidence and maintains its integrity by tracking everyone who contacts it.</p>
</details>

---

### 25. Which practice is part of maintaining chain of custody?
- [ ] Working only from the original evidence
- [ ] Letting anyone on the team handle evidence
- [ ] Labeling, cataloging, sealing, and storing items
- [ ] Storing evidence on the compromised system

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Labeling, cataloging, sealing, and storing items</p>
<p>All items are digitally tagged for ongoing documentation.</p>
</details>

---

### 26. When acquiring data from a virtual system, what should you get?
- [ ] Just the virtual machine's RAM contents
- [ ] Only the host's firmware and its OS files
- [ ] A snapshot of all its files and information
- [ ] Only a list of the users who logged into it

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> A snapshot of all its files and information</p>
<p>Acquisition obtains data from the disk, RAM, firmware, OS files, and more. Some of the data may not be on a single system.</p>
</details>

---

### 27. Which are examples of left-behind digital items to look for during acquisition?
- [ ] Clean OS images and network diagrams
- [ ] Recycle bins, browser bookmarks, and saved logins
- [ ] Hold notifications and certificates of destruction
- [ ] CVSS scores and vulnerability scan reports

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Recycle bins, browser bookmarks, and saved logins</p>
<p>Log information is another left-behind item worth collecting.</p>
</details>

---

### 28. Which section of a forensic report gives an overview of the security event?
- [ ] The summary information
- [ ] The detailed acquisition process
- [ ] The findings and analysis
- [ ] The conclusion of the report

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> The summary information</p>
<p>The report also includes a detailed explanation of the data acquisition process, the findings (an analysis of the data), and a conclusion based on that analysis. It may be used internally or in legal proceedings.</p>
</details>

---

### 29. When preserving evidence, how should analysts handle the collected data?
- [ ] Work directly on the original data
- [ ] Work from copies of the data
- [ ] Power down devices before collecting
- [ ] Analyze it once, then delete it

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Work from copies of the data</p>
<p>The data is isolated and protected so it can be analyzed, maybe years later, without any alterations. Following best practices helps ensure it's admissible in court.</p>
</details>

---

### 30. Why does evidence collection from mobile devices need special attention?
- [ ] They can be easily erased from remote locations
- [ ] They never store any data relevant to incidents
- [ ] They can't be included in a chain of custody
- [ ] They always store their data unencrypted

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> They can be easily erased from remote locations</p>
<p>Managing the collection process includes handling mobile devices quickly and carefully.</p>
</details>

---

### 31. Why has live collection become an important forensics skill?
- [ ] Live data is always admissible, while offline data isn't
- [ ] Live collection removes the need for a chain of custody
- [ ] Powering a device down always erases its storage drive
- [ ] Data may be encrypted or hard to collect after power down

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Data may be encrypted or hard to collect after power down</p>
<p>Collecting while the system is still running captures data that might otherwise be lost.</p>
</details>

---

### 32. How does e-discovery differ from digital forensics?
- [ ] E-discovery analyzes the data and determines the attacker's real intent
- [ ] E-discovery gathers data for legal process, without analysis or intent
- [ ] E-discovery only recovers deleted data from storage drives
- [ ] E-discovery is only performed during a tabletop exercise

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> E-discovery gathers data for legal process, without analysis or intent</p>
<p>E-discovery collects, prepares, reviews, interprets, and produces electronic documents required by the legal process.</p>
</details>

---

### 33. E-discovery obtains a storage drive, but it holds less data than expected. What happens next?
- [ ] The drive is returned and the case is closed
- [ ] E-discovery staff decide what the owner intended to do
- [ ] The drive is wiped and issued to a new user
- [ ] Forensics experts check for and recover deleted data

<details>
<summary>Show Answer</summary>
<p><strong>Answer:</strong> Forensics experts check for and recover deleted data</p>
<p>This shows how e-discovery and digital forensics work together.</p>
</details>
